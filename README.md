# devops19-netology

# 1.Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.|
# Выполнена команда: $ git log -p aefea
# commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545
# Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
# Date:   Thu Jun 18 10:29:58 2020 -0400

#    Update CHANGELOG.md
 
# 2.Какому тегу соответствует коммит 85024d3?
# Выполнена команда: $ git show 85024d3
# commit 85024d3100126de36331c6982bfaac02cdab9e76 (tag: v0.12.23)
# Author: tf-release-bot <terraform@hashicorp.com>
# Date:   Thu Mar 5 20:56:10 2020 +0000

#    v0.12.23

# 3.Сколько родителей у коммита b8d720? Напишите их хеши.
# Выполнена команда: $ git log -1 b8d720
# commit b8d720f8340221f2146e4e4870bf2ee0bc48f2d5 (искомый коммит)
# Merge: 56cd7859e 9ea88f22f (родители)

# 4.Перечислите хеши и комментарии всех коммитов которые были сделаны между тегами v0.12.23 и v0.12.24.#%
# Выполнена команда: $ git log v0.12.23...v0.12.24
# commit 33ff1c03bb960b332be3af2e333462dde88b279e (tag: v0.12.24)
# Author: tf-release-bot <terraform@hashicorp.com>
# Date:   Thu Mar 19 15:04:05 2020 +0000

#    v0.12.24

# commit b14b74c4939dcab573326f4e3ee2a62e23e12f89
# Author: Chris Griggs <cgriggs@hashicorp.com>
# Date:   Tue Mar 10 08:59:20 2020 -0700

#    [Website] vmc provider links

# commit 3f235065b9347a758efadc92295b540ee0a5e26e
# Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
# Date:   Thu Mar 19 10:39:31 2020 -0400

#    Update CHANGELOG.md

# commit 6ae64e247b332925b872447e9ce869657281c2bf
# Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
# Date:   Thu Mar 19 10:20:10 2020 -0400


# 5.Найдите коммит в котором была создана функция func providerSource, ее определение в коде выглядит так func providerSource(...) (вместо троеточего перечислены аргументы).
# Выполнена команда: $ git log -S 'func providerSource' --pretty=format:"%h, %an, %ad, %s"
# Найден результат по дате - 8c928e835, Martin Atkins, Thu Apr 2 18:04:39 2020 -0700, main: Consult local directories as potential mirrors of providers


# 6.Найдите все коммиты в которых была изменена функция globalPluginDirs.
# Выполнена команда: $ git log -S 'globalPluginDirs'
# commit 125eb51dc40b049b38bf2ed11c32c6f594c8ef96
# Author: Alisdair McDiarmid <alisdair@users.noreply.github.com>
# Date:   Thu May 5 10:12:00 2022 -0400

#    Remove accidentally-committed binary

#    Also add this path to .gitignore to prevent future mistakes.

# commit 22c121df8631c4499d070329c9aa7f5b291494e1
# Author: Anna Winkler <3526523+annawinkler@users.noreply.github.com>
# Date:   Tue May 3 12:28:41 2022 -0600

#    Bump compatibility version to 1.3.0 for terraform core release (#30988)

#    * Bump compatibility version to 1.3.0 for terraform core release

#    Co-authored-by: Brandon Croft <brandon.croft@gmail.com>

# commit 35a058fb3ddfae9cfee0b3893822c9a95b920f4c
# Author: Martin Atkins <mart@degeneration.co.uk>
# Date:   Thu Oct 19 17:40:20 2017 -0700

# 7.Кто автор функции synchronizedWriters?
# Выполнена команда: $ git log -S 'synchronizedWriters' --pretty=format:"%h, %an, %ad, %s"
# Найден результат - bdfea50cc, James Bardin, Mon Nov 30 18:02:04 2020 -0500, remove unused
