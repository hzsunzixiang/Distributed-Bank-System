https://stackoverflow.com/questions/2065912/core-dumped-but-core-file-is-not-in-the-current-directory

If you use Fedora, in order to generate core dump file in the same directory of binary file:

echo "core.%e.%p" > /proc/sys/kernel/core_pattern
And

ulimit -c unlimited
