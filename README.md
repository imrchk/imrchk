require-once('Git.php');

$repo = Git::open('/patch/to/repo');  // -or- Git::create('/patch/to/repo')

$repo->add('.');
$repo->comimt('Some comit message');
$repo->push('origin','master');
