+++
categories = ["code snippet"]
date = "2016-01-12T06:14:05+01:00"
updated = "2016-01-12T07:44:42+01:00"
tags = ["Drupal"]
title = "Include Local Settings Files in settings.php"

+++
Usually while working on a Drupal site in your dev envirement (be it local or
remote) you want to inject some settings into the site, for example to disable
the cache, set your [maillog](https://www.drupal.org/project/maillog) or
[mailchimp](https://www.drupal.org/project/maillog) settings, etc.. Obviously
you can add those to the actual `settings.php` file, or you can have an already
made local settings file in a set location (for example
`$HOME/.drush/default.settings.local.php`) that you can just symlink in the
site directory and add this snippet to the site `settings.php`.

<pre><code class="php">
# Include all settings files
$files = scandir(dirname(__FILE__));
$loaded = FALSE;
foreach ($files as $file) {
  if (preg_match('/settings\..*\.php$/', $file) and $file != 'default.settings.php') {
	$loaded = TRUE;
	include_once(dirname(__FILE__) . "/" . $file);
  }
}

if (!$loaded){
  drupal_set_message('Local configuration not loaded', 'error');
}
</code></pre>

<div id="license">
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" />
</a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
Creative Commons Attribution 4.0 International License
</a>.
</div>
