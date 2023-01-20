# OpenBSD

# Xorg

rcctl enable xenodm
rcctl start xenodm

# clock unsynced
rdate -s pool.ntp.org

cron
*/15 * * * * /usr/sbin/rdate -s pool.ntp.org

# upgrade
pkg_add -uvi

# ZSH encoding

export LC_ALL=C.UTF-8
export LC_CTYPE=C.UTF-8