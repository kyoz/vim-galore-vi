<div align='center'>
  <br /><br /><br />
  <img src='https://raw.githubusercontent.com/mhinz/vim-galore/master/static/images/logo-vim-galore.png' alt='vim-galore logo' />
  <br /><br /><br /><br />
  <div>
    <a href='https://github.com/mhinz/vim-galore'>English</a> |
    <a href='https://github.com/wsdjeg/vim-galore-zh_cn'>Chinese</a> |
    <a href='http://postd.cc/?s=vim-galore'>Japanese</a> |
    <a href='https://github.com/lsrdg/vim-galore'>Portuguese</a> |
    <a href='http://givi.olnd.ru/vim-galore/vim-galore-ru.html'>Russian</a>
    <div>
      <br />
      <sub>Được cấp phép theo <a href='https://creativecommons.org/licenses/by-sa/4.0'>CC BY-SA 4.0<a/>.</sub>
    </div>
  </div>
  <br /><br />
</div>

### [Giới thiệu](#giới-thiệu-1)

- [Vim là gì?](#vim-là-gì?)
- [Triết lý của Vim](#triết-lý-của-vim)
- [Những bước đầu tiên](#những-bước-đầu-tiên)
- [File cấu hình vimrc đơn giản](#file-cấu-hình-vimrc-đơn-giản)
- [Bạn đang sử dụng phiên bản Vim nào?](#bạn-đang-sử-dụng-phiên-bản-vim-nào?)
- [Cheatsheets](#cheatsheets)

### [Cơ bản](#cơ-bản)

- [Buffer, window và tab](#buffer,-window-và-tab)
- [Hiểu rõ hơn về buffer](#hiểu-rõ-hơn-về-buffer)
- [Danh sách tham số](#danh-sách-tham số)
- [Mapping lệnh](#mapping-lệnh)
- [Phím leader](#phím-leader)
- [Register](#register)
- [Ranges](#ranges)
- [Marks](#marks)
- [Completion](#completion)
- [Motions, operators, text objects](#motions-operators-text-objects)
- [Autocmds](#autocmds)
- [Changelist, jumplist](#changelist-jumplist)
- [Undo tree](#undo-tree)
- [Quickfix and location lists](#quickfix-and-location-lists)
- [Macros](#macros)
- [Colorschemes](#colorschemes)
- [Folding](#folding)
- [Sessions](#sessions)
- [Locality](#locality)

### [Usage](#usage-1)

- [Nhận hỗ trợ mà không cần kết nối mạng](#nhận-hỗ-trợ-mà-không-cần-kết-nối-mạng)
- [Getting help offline (alternative)](#getting-help-offline-alternative)
- [Getting help online](#getting-help-online)
- [Autocmds in practice](#autocmds-in-practice)
  - [User events](#user-events)
  - [Nested autocmds](#nested-autocmds)
- [Clipboard](#clipboard)
  - [Clipboard usage (Windows, macOS)](#clipboard-usage-windows-macos)
  - [Clipboard usage (Linux, BSD, ...)](#clipboard-usage-linux-bsd-)
- [Restore cursor position when opening file](#restore-cursor-position-when-opening-file)
- [Temporary files](#temporary-files)
  - [Backup files](#backup-files)
  - [Swap files](#swap-files)
  - [Undo files](#undo-files)
  - [Viminfo files](#viminfo-files)
  - [Example configuration for temporary files](#example-configuration-for-temporary-files)
- [Editing remote files](#editing-remote-files)
- [Quản lý plugin](#quan-ly-plugin)
- [Block insert](#block-insert)
- [Running external programs and using filters](#running-external-programs-and-using-filters)
- [Cscope](#cscope)
- [MatchIt](#matchit)
- [True colors](#true-colors)

### [Tips](#tips-1)

- [Go to other end of selected text](#go-to-other-end-of-selected-text)
- [Saner behavior of n and N](#saner-behavior-of-n-and-n)
- [Saner command-line history](#saner-command-line-history)
- [Saner CTRL-L](#saner-ctrl-l)
- [Disable audible and visual bells](#disable-audible-and-visual-bells)
- [Quickly move current line](#quickly-move-current-line)
- [Quickly add empty lines](#quickly-add-empty-lines)
- [Quickly edit your macros](#quickly-edit-your-macros)
- [Quickly jump to header or source file](#quickly-jump-to-header-or-source-file)
- [Quickly change font size in GUI](#quickly-change-font-size-in-gui)
- [Change cursor style dependent on mode](#change-cursor-style-dependent-on-mode)
- [Don't lose selection when shifting sidewards](#dont-lose-selection-when-shifting-sidewards)
- [Reload a file on saving](#reload-a-file-on-saving)
- [Smarter cursorline](#smarter-cursorline)
- [Faster keyword completion](#faster-keyword-completion)
- [Cosmetic changes to colorschemes](#cosmetic-changes-to-colorschemes)

### [Commands](#commands-1)

- [:global and :vglobal](#global-and-vglobal) - Execute a command on all matching lines.
- [:normal and :execute](#normal-and-execute) - The scripting dream team.
- [:redir and execute()](#redir-and-execute) - Capture command output.

### [Debugging](#debugging-1)

- [General tips](#general-tips)
- [Verbosity](#verbosity)
- [Profiling startup time](#profiling-startup-time)
- [Profiling at runtime](#profiling-at-runtime)
- [Debugging Vim scripts](#debugging-vim-scripts)
- [Debugging syntax files](#debugging-syntax-files)

### [Miscellaneous](#miscellaneous-1)

- [Tài liệu bổ sung](#tai-lieu-bo-sung)
- [Vim distributions](#vim-distributions)
- [Standard plugins](#standard-plugins)
- [Map CapsLock to Control](#map-capslock-to-control)
- [Generating HTML from buffer](#generating-html-from-buffer)
- [Easter eggs](#easter-eggs)
- [Why hjkl for navigation?](#why-hjkl-for-navigation)

### [Common problems](#common-problems-1)

- [Editing small files is slow](#editing-small-files-is-slow)
- [Editing huge files is slow](#editing-huge-files-is-slow)
- [Bracketed paste (or why do I have to set 'paste' all the time?)](#bracketed-paste-or-why-do-i-have-to-set-paste-all-the-time)
- [Delays when using escape key in terminal](#delays-when-using-escape-key-in-terminal)
- [Function search undo](#function-search-undo)

### [Technical quirks](#technical-quirks-1)

- [Newline used for NUL](#newline-used-for-nul)

### [Terminology](#terminology-1)

- [Vim script? Vimscript? VimL?](#vim-script-vimscript-viml)

### [List of colorschemes](PLUGINS.md#colorschemes-1)

### [List of plugins](PLUGINS.md)

<br>

# Giới thiệu

## Vim là gì?

[Vim](http://www.vim.org) là một trình soạn thảo văn bản có nguồn gốc lâu đời
[qed](https://en.wikipedia.org/wiki/QED_(text_editor)). Được 
[Bram Moolenaar](https://en.wikipedia.org/wiki/Bram_Moolenaar) phát hành vào 
năm 1991.

Dự án của Vim được công khai trực tuyến tại [vim.org](http://www.vim.org/index.php).

Để tải Vim: Sử dụng trình quản lý package yêu thích của bạn hoặc tải trực tiếp 
tại [vim.org](http://www.vim.org/download.php).

Bạn nên thảo luận và đặt các câu hỏi tại 
[vim_use](https://groups.google.com/forum/#!forum/vim_use) hoặc sử dụng 
IRC ([Freenode](https://freenode.net)) trong kênh của `#vim`.

Xem quá trình phát triển của Vim tại [GitHub](https://github.com/vim/vim), 
và cùng nhau thảo luận trên 
[vim_dev](https://groups.google.com/forum/#!forum/vim_dev).

Bạn cũng có thể đọc bài viết [Why, oh WHY, do those #?@! nutheads use
vi?](http://www.viemu.com/a-why-vi-vim.html) để được giải thích thêm về những 
quan niệm sai lầm phổ biến về Vim.

**Chú ý:** mình sẽ giữ nguyện một số tên gọi và khái niệm ở nguyên bản tiếng anh, 
bời vì có rất nhiều từ được sử dụng rộng rãi và phổ biến trong giới lập trình 
rồi, nếu dịch hết sang Tiếng Việt, dù bạn có hiểu nhưng sau này khi muốn cài 
thêm plugin, viết plugin, hoặc hoặc VimScript, các bạn sẽ dễ nhầm lẫn với các 
khái niệm và tên gọi đó. Hơn hết nhiều từ dịch sang Tiếng Việt đọc rất chuối :3.

## Triết lý của Vim

Vim tuân thủ triết lý chỉnh sửa theo phương thức. Điều này có nghĩa là Vim sẽ 
cung cấp nhiều chế độ và nhiều phím tắt khác nhau, ý nghĩa của các phím tắt sẽ 
được thay đổi theo từng chế độ. Bạn có thể sử dụng chế độ _normal_ để điều hướng 
các tệp tin và con trỏ chuột, sử dụng chế độ _insert_ để chèn văn bản, sử dụng 
chế độ _visual_ để chọn nhiều dùng cùng một lúc, hoặc bạn có thể sử dụng chế độ 
_command-line_ để truy cập các lệnh trong Vim, v.v. Điều này thoạt nghe thì có vẻ 
phức tạp, nhưng nó lại mạng đến một lợi thế rất lớn: đó là bạn không phải làm 
khổ các ngón tay của mình khi giữ nhiều nút trên bàn phím cùng một lúc, hầu hết 
thời gian khi bạn sử dụng Vim, bạn chỉ cần nhấn lần lượt từ phím này đến phím 
khác. Công việc càng thông dụng, thì càng ít phím phải nhấn.

Các khái niệm hoạt động tốt cùng với việc chỉnh sửa theo phương thức là 
các toán tử (operators) và chuyển động (motions). _Operators_ sẽ bắt đầu một hành 
động nhất định, ví dụ như: thay đổi, xóa hoặc chọn văn bản. Sau đó, bạn sẽ chỉ 
định vùng văn bản bạn muốn thực hiện thay đổi bằng cách sử dụng _motion_. Để thay 
đổi mọi thứ giữa các dấu ngoặc đơn, bạn có thể dùng `ci(`. Để xóa toàn bộ nội 
dung của một đoạn văn bản, chỉ cần nhấn `dap`. (Bạn không cần quá lo lắng nếu 
bạn không hiểu các ví dụ này, nội dung chi tiết sẽ được diễn giải cặn kẽ trong 
các phần sau)

Nếu bạn nhìn những người sử dụng Vim thành thạo làm việc, bạn sẽ nhận thấy rằng 
họ nói _ngôn ngữ của Vim_, cũng giống như các nghệ sĩ piano xử lý các nhạc cụ của 
họ vậy. Các thao tác phức tạp được xử lý chỉ bằng một vài phím bấm. Họ thậm chí 
còn không thèm nghĩ về nó nữa, bởi vì 
[bộ nhớ cơ bắp (muscle memory)](https://en.wikipedia.org/wiki/Muscle_memory) đã 
tiếp quản công việc thay họ.  Điều này làm giảm 
[gánh nặng nhận thức (cognitive load)](https://en.wikipedia.org/wiki/Cognitive_load) 
và giúp họ tập trung vào công việc thực sự của họ.

## Những bước đầu tiên

Vim đi kèm với một hướng dẫn tương tác (sử dụng), giúp bạn hiểu và dạy bạn 
những điều cơ bản nhất mà bạn cần biết. Bạn có thể bắt đầu nó với lệnh:

```
$ vimtutor
```

Đừng bỏ cuộc bởi vì trông nó thật nhàm chán mà hãy cố gắng vượt qua hết tất cả 
các bài tập. Các trình soạn thảo văn bản hoặc IDE mà bạn sử dụng trước đây có 
lẽ hầu hết đều không theo triết lý chỉnh sửa theo phương thức, vì vậy việc phải 
chuyển qua, chuyển lại giữa các chế độ ban đầu sẽ có đôi chút khó khăn với bạn, 
nhưng bạn càng tập luyện, càng sử dụng Vim nhiều, nó sẽ trở thành
[bộ nhớ cơ bắp (muscle memory)](https://en.wikipedia.org/wiki/Muscle_memory) 
của bạn.

Vim đã được tích hợp vào 
[Stevie](https://en.wikipedia.org/wiki/Stevie_(text_editor)), một bản sao của 
[vi](https://en.wikipedia.org/wiki/Vi), và hỗ trợ hai chế độ hoạt động khác 
nhau: "tương thích (compatible)" và "không tương thích (nocompatible)". Sử dụng 
vim ở chế độ compatible nghĩa là bạn sẽ sử dụng vi cho tất cả các thao tác, 
thay vì Vim (theo mặc định). Miễn là bạn chưa tạo file cấu hình (vimrc) hoặc 
khởi động Vim bằng cú pháp `vim -N`, chế độ tương thích chỉ là giả định, bạn 
không nên sử dụng Vim ở chế độ tương thích. Đừng nhé.

Các bước tiếp theo:

1. Tạo file cấu hình [vimrc](#file-cấu-hình-vimrc-đơn-giản) cho riêng bạn.
2. Chọn một vài [cheatsheets](#cheatsheets) để chuẩn bị sử dụng cho những tuần 
đầu tiên sử dụng Vim.
3. Đọc qua phần [cơ bản](#cơ-bản) để biết được những điều khó tin mà Vim có 
thể làm.
4. Học theo nhu cầu sử dụng! Bạn sẽ không bao giờ hết được Vim. Nếu bạn gặp bất 
kì vấn đề nào, chỉ cần tìm kiếm nó trên mạng. Vấn đề mà bạn mắc phải đã được 
giải quyết sẵn trên mạng. Vim đi kèm với một bộ tài liệu tuyệt vời, và việc bạn 
phải biết cách sử dụng, tra khảo nó là một điều bắt buộc: 
[Nhận hỗ trợ mà không cần kết nối mạng](#nhận-hỗ-trợ-mà-không-cần-kết-nối-mạng).
5. Đọc qua [tài liệu bổ sung](#tài-liệu-bổ-sung).

Lời khuyên cuối cùng: Vui lòng học cách sử dụng Vim đúng cách trước khi bạn bắt 
đầu thêm thắt các loại [plugin](#quản-lý-plugin) mà bạn không hề biết rằng 
những tính năng của các plugin đó đã sẵn có trong Vim.

## File cấu hình vimrc đơn giản

Bạn có thể đặt file cấu hình vimrc của bạn ở `~/.vimrc` hoặc để quản lý tốt 
hơn, bạn có thể phân chia nó ra và đặt nó vào `~/.vim/vimrc`. Việc tách các 
file cấu hình ra sẽ giúp bạn dễ dàng quản lý các phiên bản cho từng bộ cấu hình 
của mình, và tải nó lên mạng, giả sử như Github chẳng hạn.

Bạn có thể tìm thấy nhiều file cấu hình `vimrc đơn giản` trên mạng, ví dụ như 
những file cấu hình của tôi, mặc dù trông chúng không được đơn giản cho lắm, 
nhưng nó sẽ cung cấp cho bạn một bộ cài đặt, cấu hình ổn định mà tôi cho là 
rất hữu ích để bạn bắt đầu.

Cuối cùng, bạn vẫn phải đọc qua hết tất cả các cài đặt có trong file cấu hình 
và tự quyết định sẽ cấu hình như thế nào cho chính bản thân mình. :-)

Xem file cấu hình ở đây nhé: [vimrc](static/minimal-vimrc.vim)

Trong trường hợp bạn quan tâm, đây là 
[file cấu hình của tôi](https://github.com/kyoz/neovim).

**MẸO NHỎ**: Hầu hết những người làm ra plugin đều chia sẻ file cấu hình vimrc 
của họ trên Github (thường thì họ sẽ đặt trong repo có tên "dotfiles" hoặc 
"vim-config"), vì vậy bất cứ khi nào bạn tìm thấy một plugin bạn thích, bạn hãy 
xem qua GitHub của tác giả làm ra plugin đó và xem qua các repo để tham khảo 
các file cấu hình của họ.

## Bạn đang sử dụng phiên bản Vim nào?

Dùng lệnh `:version` trong vim sẽ cung cấp cho bạn tất cả các thông tin bạn cần 
biết về phiên bản Vim mà bạn đang sử dụng.

Dòng đầu tiên cho bạn biết phiên bản Vim bạn đang sử dụng được biên dịch khi 
nào, cũng như phiên bản của nó, ví dụ: 7.4. Dòng tiếp theo có cấu trúc 
`Included patches: 1-1051`, là bản patch của Vim. Do đó, phiên bản Vim chính 
xác của bạn là 7.4.1051.

Dòng tiếp theo có thể là `Tiny version without GUI (Phiên bản tối giản với giao diện)` 
hoặc `Huge version with GUI (Phiên bản đầy đủ với giao diện)` . Thông tin chúng 
muốn đề cập là liệu Vim của bạn có hỗ trợ giao diện (GUI) hay không, ví dụ: để 
khởi động `gvim` từ shell hoặc chạy `:gui` từ Vim trong terminal. Một thông tin 
quan trọng khác là `Tiny` và `Huge`. Vim phân biệt giữa các tập tính năng bằng 
các tên gọi như `tiny`, `small`, `normal`, `big`, và `huge`, mỗi tập sẽ cũng 
cấp những tính năng khác nhau cho Vim của bạn.

Hầu hết các phiên bản của vim khi bạn xem `:version` sẽ đều hiển thị các tính 
năng đang được hay không được tích hợp sẵn. Ví dụ `+clipboard` nghĩa là tính 
năng clipboard được tính hợp sẵn, `-clipboard` nghĩa là tính năng clipboard 
không được tính hợp sẵn trong phiên bản Vim hiện tại của bạn.

Một số tính năng của Vim cần được biên dịch để có thể hoạt động. Ví dụ để chạy 
được lệnh `:prof`, bạn sẽ cần phiên bản Vim với tập tính năng `Huge`, bởi vì 
tập đó có sẵn tính năng `+profile`.

Nếu không rành, hoặc giả sử bạn cài đặt Vim từ trình quản lý package, hãy đảm 
bảo bạn đã cài đặt các gói có tên `vim-x`, `vim-x11`, `vim gtk`, `vim-gnome` 
hoặc tương tự, vì các gói này thường đi kèm với bộ tính năng khổng lồ.

Bạn cũng có thể kiểm tra phiên bản hoặc các tính năng của Vim bằng các lập 
trình với lệnh như sau:

```vim
" Chạy lệnh gì nó nếu phiên bản của Vim mới hơn hoặc bằng 7.4.42
" Và phải có +profile
if (v:version > 704 || v:version == 704 && has('patch42')) && has('profile')
  " do stuff
endif
```

Để hiểu rõ hơn bạn có thể dùng các lệnh sau để tra cứu thêm thông tin:

```
:h :version
:h feature-list
:h +feature-list
:h has-patch
```

## Cheatsheets

- http://people.csail.mit.edu/vgod/vim/vim-cheat-sheet-en.png
- https://cdn.shopify.com/s/files/1/0165/4168/files/preview.png
- http://michael.peopleofhonoronly.com/vim/vim_cheat_sheet_for_programmers_screen.png
- http://www.rosipov.com/images/posts/vim-movement-commands-cheatsheet.png

Hoặc bạn cũng có thể mở nhanh một bảng cheatsheet ngay bên trong vim: 
[vim-cheat40](https://github.com/lifepillar/vim-cheat40).

# Cơ bản

## Buffer, window và tab

Vim là một trình soạn thảo văn bản. Mỗi khi văn bản được hiển thị, văn bản sẽ 
là một phần của **buffer (bộ nhớ đệm)**. Mỗi tệp sẽ được mở trong buffer của riêng 
nó. Các plugin sẽ hiển thị nội dung của chúng trong buffer của riêng từng 
plugin, vv.

Các buffer có rất nhiều thuộc tính, ví dụ: văn bản có bạn có thể chỉnh sửa 
(modifiable) được hay không, hoặc liệu nó có được liên kết với một file nào đó 
hay không, và do đó nó cần được đồng bộ với ổ đĩa khi bạn lưu văn bản.

**Các window** là các cửa sổ (khung hiển thị) _để hiển thị_ các buffer. Nếu bạn muốn 
xem nhiều file cùng một lúc hoặc nhiều vị trí các nhau trên một file, bạn sẽ 
phải sử dụng window.

Và làm ơn, đừng gọi chúng là _splits (chia cửa sổ)_ . Bạn có thể chia một window 
làm 2, nhưng điều đó không khiến chúng trở thành _splits_.

Window có thể được chia theo chiều ngang hoặc chiều dọc, chiều dài và rộng của 
chúng cũng có thể được thay đổi. Do đó, bạn có thể sử dụng bất kì cách phân 
chia cửa sổ nào mà bạn thích nhất.

Tab (hay còn được gọi là Tab page), là tập hợp của các cửa sổ. Vì vậy, nếu bạn 
muốn sử dụng nhiều bố cục cửa sổ khác nhau, hãy sử dụng các tab.

Tóm lại, nếu bạn khởi động Vim mà không có bất kì arguments (tham số) nào, bạn 
sẽ chỉ có một tab, bên trong tab là một window đang hiển thị một buffer.

Ngoài ra, tất cả các buffer đều khả dụng trong toàn bộ trình soạn thảo Vim, và 
bạn có thể truy cập mọi buffer từ bất kì tab nào.

## Hiểu rõ hơn về buffer

Bạn có thể khởi động Vim bằng các chạy lệnh `vim file-1`. Nội dung của file sẽ 
được load vào buffer. Nội dung của buffer chỉ được đồng bộ hóa vào ổ đĩa (ghi 
vào file) khi bạn lưu nó bằng lệnh bên trong Vim.

Bởi vì buffer cũng được hiển thị bên trong window, nó cũng là một **active buffer 
(buffer đang hoạt động)**. Bây giờ nếu bạn load một file khác với lệnh `e file-2`, 
`file-1` sẽ trở thành **hidden buffer (buffer ẩn)** và `file-2` sẽ trở thành 
`active buffer`.

Cả hai buffer đều được **liệt kê** trong danh sách buffer, do đó, khi bạn dùng lệnh 
`:ls` để hiển thị danh sách buffer, chúng đều sẽ được hiển thị trong danh sách. 
Buffer của các plugin hoặc các buffer trợ giúp (help buffer) thông thường sẽ 
không được hiển thị trong danh sách buffer, bởi vì chúng không đại diện cho các 
file thông thường mà bạn hay chỉnh sửa bằng các trình soạn thảo văn bản. Để 
hiển thị tất cả buffer (kể các các buffer ẩn) bạn có thể sử dụng lệnh `:ls!`.

**Unnamed buffers (các buffer không tên)**, cũng thường được sử dụng bởi các plugin, 
chúng là các buffer không có liên kết và cũng không đại diện cho một file cụ 
thể nào cả. Ví dụ: dùng lệnh `:enew` sẽ tạo ra một buffer tạm không có tên 
(unnamed buffer). Bạn có thể gõ vài dòng chữ vào đó và ghi nó vào đĩa bằng cách 
chỉ định một file để liên kết, ví dụ: `:w /tmp/foo`, nội dung bạn vừa gõ sẽ 
được lưu vào file `/tmp/foo` và buffer vô danh vừa tạo sẽ trở thành một buffer 
bình thường.

## Danh sách tham số

[Danh sách buffer toàn cục (global buffer list)](#buffer,-window-và-tab) là một 
đặc trưng của Vim. Trước đây, bên trong vi, những thứ này chỉ được sử dụng như 
là các tham số, trong khi đó chúng lại có sẵn bên trong Vim.

Mỗi file (tên file) được cung cấp cho Vim bằng lệnh, đều được ghi nhớ trong 
danh sách tham số (argument list). Trong Vim, có thể có nhiều danh sách tham 
số khác nhau: theo mặc định, tất cả các tham số được đưa vào danh sách tham số 
toàn cục (global argument list), nhưng bạn có thể sử dụng lệnh `:arglocal` để 
tạo một danh sách tham số cục bộ (local) cho window.

Bạn có thể liệt kê danh sách tham số với lệnh `:args`. Chuyển đổi qua lại giữa 
các file từ danh sách tham số với lệnh `:next`, `:before`, `:previous`, `:first`,
`:last` và các lệnh khác. Hoặc bạn cũng có thể thay thế file đó với file khác 
với lệnh `:argadd`, `:argdelete` hoặc `:args` với một danh sách các file.

Việc sử dụng buffer hoặc danh sách tham số để làm việc với các file là tùy 
thuộc vào sở thích của bạn. Thông thường tôi thấy mọi người chỉ sử dụng danh 
sách buffer.

Tuy nhiên, có một trường hợp bạn cần phải sử dụng danh sách đối số để xử lý. Ví 
dụ: xử lý hàng loạt với lệnh `:argdo`!. Đây làm một ví dụ đơn giản:

```vim
:args **/*.[ch]
:argdo %s/foo/bar/ge | update
```

Các lệnh trên sẽ thay thế tất cả các chữ "foo" thành "bar" trong tất cả các 
file C và header file của chúng trong thư mục hiện tại.

Xem thêm: `:h argument-list`

## Mapping lệnh

Bạn có thể định nghĩa các mapping của mình với danh sách các lệnh `:map`. Mỗi 
lệnh trong danh sách các lệnh đó sẽ định nghĩa một mapping cho một chế độ (mode) 
nhất định. Về mặt kĩ thuật, Vim đi kèm với 12 chế độ, 6 trong số đó chúng ta có 
thể sử dụng được mapping. Ngoài ra, một số lệnh hoạt động trên nhiều chế độ 
cùng một lúc.

| Đệ quy    | Không đệ quy  | Bỏ mapping | Chế độ                           |
|-----------|---------------|------------|----------------------------------|
| `:map`    | `:noremap`    | `:unmap`   | normal, visual, operator-pending |
| `:nmap`   | `:nnoremap`   | `:nunmap`  | normal                           |
| `:xmap`   | `:xnoremap`   | `:xunmap`  | visual                           |
| `:cmap`   | `:cnoremap`   | `:cunmap`  | command-line                     |
| `:omap`   | `:onoremap`   | `:ounmap`  | operator-pending                 |
| `:imap`   | `:inoremap`   | `:iunmap`  | insert                           |

Ví dụ: lệnh sau đây sẽ map phím `space` cho chế độ normal

```vim
:nmap <space> :echo "foo"<cr>
```

Bỏ mapping của phím vừa map bằng lệnh `:nunmap <space>`.

Để biết thêm một số chế độ phổ biến khác (hoặc sự kết hợp của chúng), bạn có 
thể xem `:h map-modes`.

Càng học bạn sẽ càng thấy Vim tuyệt vời. Chỉ có một vấn đề khá khó hiểu với 
những người mới bắt đầu, `:nmap` có tính _đệ quy_ !. Đúng vậy, vế phải của lệnh 
sẽ nhận các lệnh mà bạn muốn map.

Vì vậy, nếu bạn muốn map một lệnh đơn giản ghi ra màn hình chữ "Foo", dùng lệnh:
So you defined a mapping that simply echoes "Foo":

```vim
:nmap b :echo "Foo"<cr>
```

Nhưng nếu bạn muốn map hành vi mặc định của phím `b` vừa map cho một phím khác (
di chuyển con trỏ về 1 từ đứng trước từ hiện tại) thì sao?. Hãy dùng lệnh:

```vim
:nmap a b
```

Nếu bạn nhấn nút <kbd>a</kbd>, chúng ta nghĩ là con trỏ sẽ nhảy đến từ đứng 
trước từ hiện tại, nhưng thay vào đó, "Foo" sẽ được in ra trong dòng lệnh! Bởi 
vì chúng ta đã map phím `b` cho một hành động khác rồi, đó là `:echo "Foo"<cr>`.

Cách thích hợp để giải quyết vấn đề này là sử dụng mapping _không đệ quy_ 
(_non-recursive_ mapping):

```vim
:nnoremap a b
```

Quy tắc: Luôn sử dụng mapping không đệ quy (non-recursive mapping) trừ khi bạn 
biết bạn đang làm gì.

Tra cứu các mapping mà bạn đã map bằng cách dùng lệnh `:nmap`. Lệnh `:nmap` sẽ 
liệt kê tất cả các mapping normal và `:nmap <leader>` sẽ liệt kê tất cả các 
mapping bắt đầu mới mapleader (Phím leader mặc định, bạn có thể thay đổi phím 
này, chi tiết sẽ được trình bày trong phần sau).

Nếu bạn muốn vô hiệu hóa một mapping, hãy map chúng thành kí tự đặc biệt `<nop>`
, ví dụ: `:noremap <left> <nop>`.

Xem thêm:

    :h key-notation
    :h mapping
    :h 05.3

## Phím leader

Phím leader có thể sử dụng chung với các mapping của bạn, giúp bạn thao tác đơn 
giản và nhanh chóng hơn. Mặc định, phím leader sẽ là `\`;

```vim
nnoremap <leader>h :helpgrep<space>
```

Sau khi map với lệnh trên, bạn có thể nhấn trên bàn phím lần lượt 2 phím 
<kbd>/</kbd><kbd>h</kbd> để chạy lệnh `:helpgrep<space>`. Ngoài phím leader, 
bạn cũng có thể map với phím cách (space) bằng cách thay `<leader>` bằng 
`<space>`.

```vim
let mapleader = ' '
nnoremap <leader>h :helpgrep<space>
```

Ngoài `<leader>`` và `<space>`, bạn còn có thể sử dụng `<localleader>`.
`<localleader>` là một bản sao cục bộ của `<leader>` được sử dụng để map các 
phím cho một buffer. Ví dụ: plugin filetype-specific cũng sử dụng `\` làm phím 
leader mặc định.

Lưu ý: Bạn cần phải cấu hình các leader trước khi tiến hành định nghĩa các 
mapping của mình. Tất cả các mapping đã được định nghĩa trước khi bạn định 
nghĩa các mapleader đều đã có hiệu lực, chúng sẽ không thay đổi vì bạn định 
nghĩa mapleader sau chúng. `:nmap <leader>` sẽ liệt kê tất cả các mapping với 
mapleader đã được áp dụng, bạn nên dùng lệnh này để kiểm tra lại các mapping 
của mình.

Xem thêm `:h mapleader` và `:h maplocalleader` để biết thêm chi tiết.

## Register

Registers (Bộ đăng ký, thanh ghi) là nơi lưu trữ các thao tác trên văn bản của 
bạn. Việc bạn sao chép một đoạn văn bản vào register được gọi là **yanking** và 
việc bạn trích xuất dữ liệu từ register được gọi là **pasting**.

Vim cung cấp cho bạn các register sau:

| Loại                | Kí tự                  | Được nhập bởi? | Không được chỉnh sửa? | Contains text from? |
|---------------------|------------------------|----------------|-----------------------|---------------------|
| Unnamed             | `"`                    | vim            | [ ]                   | Thông tin sao chép hoặc xóa gần nhất. (`d`, `c`, `s`, `x`, `y`) |
| Numbered            | `0` to `9`             | vim            | [ ]                   | register `0`: Lần sao chép gần nhất. register `1`: Lần xóa gần nhất. register `2`: Lần xóa gần thứ nhì. Và cứ như vậy. Các register từ `1`-`9` không được phép chỉnh sửa [queue](https://en.wikipedia.org/wiki/Queue_(abstract_data_type)). |
| Small delete        | `-`                    | vim            | [ ]                   | Lần xóa gần nhất mà có ít hơn 1 dòng. |
| Named               | `a` to `z`, `A` to `Z` | user           | [ ]                   | Nếu bạn muốn sao chép vào register `a`, bạn có thể thay thế nội dung của nó. Nếu bạn muốn sao chép vào register `A`, bạn thêm nó vào sau nội dung của register `a`. |
| Read-only           | `:`, `.`, `%`          | vim            | [x]                   | `:`: Lệnh bạn dùng cuối cùng, `.`: Những từ gần nhất bạn thêm vào, `%`: Tên file của buffer hiện tại. |
| Alternate buffer    | `#`                    | vim            | [ ]                   | Những buffer được truy cập gần nhất của window hiện tại. Xem `:h alternate-file` |
| Expression          | `=`                    | user           | [ ]                   | Đánh giá biểu thức VimL đã được sao chép. Ví dụ, nhập lệnh sao đây trong chế độ insert: `<c-r>=5+5<cr>` và "10" sẽ được chèn vào buffer. |
| Selection           | `+`, `*`               | vim            | [ ]                   | `*` và `+` là register [clipboard](#clipboard). |
| Drop                | `~`                    | vim            | [x]                   | Lần kéo thả gần nhất. |
| Black hole          | `_`                    | vim            | [ ]                   | Nếu bạn không muốn bất kì register nào khác bị ảnh hưởng. Ví dụ, lệnh `"_dd` sẽ xóa dòng hiện tại mà không thay đổi (ảnh hưởng) đến các register `"`, `1`, `+`, `*`. |
| Last search pattern | `/`                    | vim            | [ ]                   | Pattern gần nhất được sử dụng vơi `/`, `?`, `:global`, etc. |

Each register that is not readonly can be set by the user:
Mỗi thanh ghi không bị giới hạn ghi chép (readonly), có thể được thiết lập bởi 
người dùng:

```vim
:let @/ = 'register'
```

Sau đó, phím <kbd>n</kbd> sẽ di chuyển con trỏ đến lần xuất hiện tiếp theo của 
"register".

Có rất nhiều trường hợp ngoại lệ khi các thanh ghi được lấp đầy một cách âm thầm,
do đó, để chắc ăn, bạn nên đọc thêm `:h registers`.

Sao chép với `y` và dán với `p`/`P`, nhưng hãy nhớ rằng Vim phân biệt giữa các 
lựa chọn trực quan theo chiều của ký tự, và theo dòng. Xem thêm `:h linewise`.

**Ví dụ: sao chép dòng**

`yy` (hoặc `Y`) sẽ sao chép dòng hiện tại. Sau đó, bạn di chuyển con trỏ đến 1 
nơi nào khác tùy ý, dùng `p` để dán nội dung đã sao chép bên dưới dòng hiện 
tại, `P` để dán bên trên dòng hiện tại.

**Ví dụ: sao chép chữ**

Sao chép từ đầu tiên với `0yw`, sau đó bạn di chuyển con trỏ đến một nơi nào 
khác, dán từ vừa sao chép phía sau con trỏ của dòng hiện tại với phím `p` và 
phía trước con trỏ với phím `P`;

**Ví dụ: đặt tên cho register**

Lệnh `"aY` sẽ sao chép dòng hiện tại vào register `a`. Di chuyển sang một dòng 
khác. Lệnh `"AY` sẽ chèn dòng hiện tại vào phía cuối của register `a`.

Tôi khuyên bạn nên thử với tất cả các thanh ghi này một chút và liên tục dùng 
lệnh `:reg` để kiểm tra những gì đang thực sự diễn ra.

**Sự thật thú vị**: Trong Emacs "yanking" (sao chép) lại có nghĩa là pasting (dán)
(hoặc chèn lại vào văn bản đã bị xóa trước đó), chứ không phải mang nghĩa 
copying (sao chép).

## Ranges

Ranges (phạm vi) khá là dễ hiểu, những hầu hết các Vimmers đều không biết về 
chức năng đầy đủ của chúng.

- Rất nhiều lệnh đều có phạm vi (ranges).
- Một địa chỉ sẽ chỉ định một dòng nhất định.
- Một range có thể là một địa chỉ duy nhất hoặc một cặp địa chỉ được phân cách 
bởi `,` hoặc là `;`.
- Ranges cho biết cách lệnh nên thực thi trên dòng nào.
- Hầu hết các lệnh chỉ hoạt động trông dòng hiện tại theo mặc định. Các trường 
hợp đáng chú ý có thể kể đến là `:write` và `:global`, chúng sẽ hoạt động trên 
tất cả các dòng.

Việc sử dụng các range khá là trực quan, đây là một số ví dụ (lệnh `:d`
là viết tắt của `:delete`):

| Lệnh     | Các dòng sẽ thực thi lệnh |
|----------|----------------|
| `:d`     | Dòng hiện tại. |
| `:.d`    | Dòng hiện tại. |
| `:1d`    | Dòng đầu tiên. |
| `:$d`    | Dòng cuối. |
| `:1,$d`  | Tất cả các dòng. |
| `:%d`    | Tất cả các dòng (cú pháp ngắn gọn cho lệnh `1,$`). |
| `:.,5d`  | Dòng hiện tại tới dòng thứ 5. |
| `:,5d`   | Cũng là dòng hiện tại tới dòng thứ 5. |
| `:,+3d`  | Dòng hiện tại và 3 dòng tiếp theo. |
| `:1,+3d` | Dòng đầu tiên tới dòng hiện tại, và thêm 3 dòng sau đó. |
| `:,-3d`  | Dòng hiện tại và 3 dòng cuối. (Vim sẽ cảnh báo bạn, vì đây là phạm vi đảo ngược.) |
| `:3,'xdelete` | Dòng thứ 3 cho tới dòng được [đánh dấu](#đánh-dấu) x. |
| `:/^foo/,$delete` | Từ dòng tiếp theo, bắt đầu với từ "foo" cho tới hết file. |
| `:/^foo/+1,$delete` | Từ dòng kế tiếp của dòng bắt đầu với "foo" cho tới hết file. |

Lưu ý là thay vì dùng `,`, `;` có thể được dùng như là dấu phân cách. Sự khác 
biệt là trong trường hợp của công thức `from,to`, thì _to_ là chỉ cho dòng hiện 
tại, nhưng khi dùng công thức `from;to`, _to_ ở đây có liên quan đến địa chỉ 
của _from_!. Giả sử bạn đang ở dòng 5, `:1;+1d` sẽ chỉ xóa dòng 1 và 2.

Địa chỉ `/` có thể được đặt trước bằng một địa chỉ khác. Điều này cho phép bạn 
_gộp các pattern_ lại với nhau. Ví dụ:

```vim
:/foo//bar//quux/d
```

Lệnh trên sẽ xóa dòng đầu tiên có chứa "quux" sau dòng đầu tiên chứa "bar" sau 
dòng đầu tiên có chứa "foo" kể từ sau dòng hiện tại.

Đôi khi Vim tự động thêm một ranges vào trước dòng lệnh của bạn. Ví dụ: bắt 
đầu lựa chọn nhiều dòng với chế độ visual bằng lệnh `V`, chọn một số dòng bạn 
thích và nhập `:`. Dòng lệnh sẽ được điền với ranges `'<,'>`, có nghĩa là lệnh 
bạn chuẩn bị thực thi sẽ được áp dụng cho các dòng đã chọn trước đó. (Đây cũng 
là lý do tại sao đôi khi bạn thấy các mapping như là 
`:vnoremap foo :<c-u>command`. Ở đây `<c-u>` được sử dụng để loại bỏ ranges, 
bởi vì Vim sẽ quăng lỗi khi bạn cho ranges vào một lệnh không hỗ trợ ranges.

Một ví dụ khác nữa là sử dụng `!!` ở chế độ normal. Thao tác này sẽ tự động 
điền `:.!` vào dòng lệnh của bạn. Nếu bạn điền tiếp theo sau bởi một dòng lệnh,
hay ứng dụng bên ngoài, đầu ra của dòng lệnh, ứng dụng đó sẽ thay thế cho dòng 
hiện tại. Vì vậy, bạn có thể thay thế đoạn văn hiện tại bằng đầu ra của lệnh 
`ls` bằng cách sử dụng: `:?^$?+1,/^$/-1!ls`. Thật tuyệt.

Xem thêm:

```
:h cmdline-ranges
:h 10.3
```

## Marks

Bạn có thể sử dụng marks (đánh dấu) để ghi nhớ một vị trí, đó là vị trí dòng và 
cột bên trong một file.

| Marks | Được đặt bởi.. | Công dụng |
|-------|----------|-------|
| `a` - `z` | Người dùng | Chỉ khả dụng cục bộ trong một file. Chuyển đến một mark được đánh dấu bằng chữ viết thường nghĩa là chuyển con trỏ qua lại trong một file. |
| `A` - `Z` | Người dùng | Khả dụng toàn cục, cho tất cả các file. Còn được gọi là các _file mark__. Chuyển cho trỏ đến một marker được đánh dấu bằng chữ viết hoa có thể nhảy sang một buffer khác buffer hiện tại. |
| `0` - `9` | viminfo | `0` là vị trí khi file viminfo được ghi lần cuối. Trong thực tế, điều này có nghĩa là khi Vim được đóng lần cuối. `1` là vị trí khi Vim kết thúc lần gần thứ 2, và cứ thế cho các số tiếp theo. |

Đặt `'`/`g'` hoặc `` ` ``/`` g` `` trước một mark để tạo một cử chỉ (motion).

Sử dụng `mm` để ghi nhớ vị trí hiện tại với mark "m". Di chuyển xung quanh tệp 
và sau đó quay lại với `'m` (ký tự đầu tiên không phải khoảng trống trên 1 dòng) 
hoặc `` `m `` (vị trí cột chính xác đã đánh mark).
Các mark được đánh dấu bằng chữ thường sẽ được ghi nhớ khi bạn thoát Vim, nếu 
bạn yêu cầu file viminfo của mình làm như vậy, xem thêm `:h viminfo-'`.

Sử dụng `mM` để ghi nhớ vị trí hiện tại với mark "M". Chuyển sang buffer khác 
và quay lại vị trí vừa đánh dấu với `'M` hoặc `` `M ``.

Các cử chỉ khác:

| Cử chỉ           | Nhảy đến.. |
|------------------|-----------|
| `'[`, `` `[ ``   | Dòng hoặc ký tự đầu tiên của văn bản đã thay đổi hay được sao chép trước đó. |
| `']`, `` `] ``   | Dòng hoặc ký tự cuối cùng của văn bản đã thay đổi hay được sao chép trước đó. |
| `'<`, `` `< ``   | Dòng bắt đầu hoặc ký tự của các lựa chọn được chọn trong chế độ visual lần gần nhất. |
| `'>`, `` `> ``   | Dòng kết thúc hoặc ký tự của các lựa chọn được chọn trong chế độ visual lần gần nhất. |
| `''`, ``` `` ``` | Vị trí mà bạn vừa từ đó nhảy đến. |
| `'"`, `` `" ``   | Ví trí khi bạn thoát buffer lần gần nhất. |
| `'^`, `` `^ ``   | Vị trí bạn thực hiện chèn kí tự lần gần nhất. |
| `'.`, `` `. ``   | Vị trí bạn thực hiện thay đổi lần gần nhất. |
| `'(`, `` `( ``   | Bắt đầu câu hiện tại. |
| `')`, `` `) ``   | Kết thúc của câu hiện tại. |
| `'{`, `` `{ ``   | Bắt đầu của đoạn văn bản hiện tại. |
| `'}`, `` `} ``   | Kết thúc của đoạn văn bản hiện tại. |

Các mark đánh dấu cũng có thể được sử dụng trong một [range](#ranges). Bạn hẳn 
là đã thấy điều này trước đây và tự hỏi ý nghĩa của nó là gì: Chọn một số đoạn 
văn bản bạn thích ở chế độ visual và nhấn `:`, dòng lệnh sẽ hiển thị, và được 
thêm sẵn vào phía trước như thế này `:'<,'>`, có nghĩa là lệnh sau sẽ nhận được 
một phạm vi mà bạn đã chọn với chế độ visual.

Sử dụng `:marks` để liệt kê tất cả mark mà bạn đã đánh dấu. Đọc thêm tất cả mọi 
thứ về mark trong `:h mark-motions`.

## Completion

Vim provides many kinds of insert mode completions. If there are multiple
matches, a popup menu will let you navigate to the match of your choice.

Typical kinds of completion are tags, functions from imported modules or
libraries, file names, dictionary or simply words from the current buffer.

Vim provides a mapping for each kind of completion and they all start with
`<c-x>` (remember to use them in insert mode):

| Mapping | Kind | Help         |
|---------|------|--------------|
| `<c-x><c-l>` | whole lines | `:h i^x^l` |
| `<c-x><c-n>` | keywords from current file | `:h i^x^n` |
| `<c-x><c-k>` | keywords from `'dictionary'` option | `:h i^x^k` |
| `<c-x><c-t>` | keywords from `'thesaurus'` option | `:h i^x^t` |
| `<c-x><c-i>` | keywords from current and included files | `:h i^x^i` |
| `<c-x><c-]>` | tags | `:h i^x^]` |
| `<c-x><c-f>` | file names | `:h i^x^f` |
| `<c-x><c-d>` | definitions or macros | `:h i^x^d` |
| `<c-x><c-v>` | Vim commands | `:h i^x^v` |
| `<c-x><c-u>` | user defined (as specified in `'completefunc'`) | `:h i^x^u` |
| `<c-x><c-o>` | omni completion (as specified in `'omnifunc'`) | `:h i^x^o` |
| `<c-x>s`     | spelling suggestions | `:h i^Xs` |

People might be confused about the difference between user defined completion
and omni completion, but technically they do the same thing. They take a
function that inspects the current position and return a list of suggestions.
User defined completion is defined by the user for their own personal purposes.
(Surprise!) It could be anything. Omni completion is meant for filetype-specific
purposes, like completing struct members or class methods, and is often set by
filetype plugins.

Vim also allows for completing multiple kinds at once by setting the
`'complete'` option. By default that option includes quite a lot, so be sure to
trim it to your taste. You can trigger this completion by using either `<c-n>`
(next) and `<c-p>` (previous), which also happen to be the keys used for
choosing entries in the popup menu. See `:h i^n` and `:h 'complete'` for more on
this.

Be sure to check out `:h 'completeopt'` for configuring the behaviour of the
popup menu. The default is quite sane, but I prefer adding "noselect" as well.

Help:

```
:h ins-completion
:h popupmenu-keys
:h new-omni-completion
```

## Motions, operators, text objects

**Motions** move the cursor. You all know `h`/`j`/`k`/`l`. Or `w` and `b`. Even
`/` is a motion. They also take a count. `2?the<cr>` jumps to the second last
occurrence of "the".

See `:h navigation` and everything below for all available motions.

**Operators** act on a region of text, e.g. `d`, `~`, `gU`, `>` to name just a
few. They get used in two contexts, either in normal or visual mode. In normal
mode, operators come first followed by a motion, e.g. `>j`. In visual mode,
operators simply act on the selection, e.g. `Vjd`.

Like motions, operators take a count, e.g. `2gUw` makes the rest of the current
word and the next one uppercase. Since motions and operators take counts,
`2gU2w` works just as well and executes `gU2w` twice.

See `:h operator` for all available operators. Use `:set tildeop` to make `~`
act as an operator.

**Text objects** act on the surrounding area, opposed to motions that act into
one direction. Actually they work on objects, e.g. a whole word, a whole
sentence, everything between parentheses, and so on.

Text objects can't be used to move the cursor in normal mode, because even the
most-skilled cursors can't jump into two directions at the same time. It works
in visual mode though, because then one side of the object is already selected
and the cursor simply jumps to the other side.

Text objects start with either `i` (think _inner_) or `a` (think _around_)
followed by a character denoting the object. With `i` it only acts on the object
itself, with `a` on the object plus trailing whitespace. E.g. `diw` deletes the
current word and `ci(` changes everything between parentheses.

Text objects take a count. Imagine `((( )))` and the cursor on or between the
most inner parentheses, then `d2a(` will remove the 2 inner pairs of parentheses
and everything in between.

See `:h text-objects` for all available text objects.

## Autocmds

You can trigger an action after many events in Vim, such as a buffer being
saved or Vim having started up, by so-called _autocmds_.

Vim relies extensively on autocmds. Don't believe me? Check `:au`, but don't let
the output overwhelm you. These are all the autocmds that are in effect right
now!

See `:h {event}` for a quick overview of all available events and `:h
autocmd-events-abc` for more details.

A typical example would be filetype-specific settings:

```vim
autocmd FileType ruby setlocal shiftwidth=2 softtabstop=2 comments-=:#
```

But how does a buffer even know that it contains Ruby code? Because another
autocmd detected it as that and set the filetype accordingly which again
triggered the `FileType` event.

One of the first things everyone adds to their vimrc is `filetype on`. This
simply means that `filetype.vim` is read at startup which sets autocmds for
almost all filetypes under the sun.

If you're brave enough, have a look at it: `:e $VIMRUNTIME/filetype.vim`. Search
for "Ruby" and you'll find that Vim simply uses the file extension `.rb` to
detect Ruby files:

**NOTE**: Autocmds of the same event are executed in the order they were
created. `:au` shows them in the correct order.

```vim
au BufNewFile,BufRead *.rb,*.rbw  setf ruby
```

The `BufNewFile` and `BufRead` events in this case are hardcoded in the C
sources of Vim and get emitted everytime you open a file via `:e` and similar
commands. Afterwards all the hundreds of filetypes from `filetype.vim` are
tested for.

Putting it in a nutshell, Vim makes heavy use of events and autocmds but also
exposes a clean interface to hook into that event-driven system for
customization.

Help: `:h autocommand`

## Changelist, jumplist

The positions of the last 100 changes are kept in the **changelist**. Several
small changes on the same line will be merged together, but the position will be
that of the last change nevertheless (in case you added something in the middle
of the line).

Every time you jump, the position _before_ the jump is remembered in the
**jumplist**. A jumplist has up to 100 entries. Each window has its own
jumplist. When you split a window, the jumplist is copied.

A jump is one of the following commands: `'`, `` ` ``, `G`, `/`, `?`, `n`, `N`,
`%`, `(`, `)`, `[[`, `]]`, `{`, `}`, `:s`, `:tag`, `L`, `M`, `H` and commands
that start editing a new file.

| List       | List all entries | Go to older position | Go to newer position |
|------------|------------------|----------------------|----------------------|
| jumplist   | `:jumps`         | `[count]<c-o>`       | `[count]<c-i>`       |
| changelist | `:changes`       | `[count]g;`          | `[count]g,`          |

When you list all entries, a marker `>` will be used to show the current
position. Usually that will be below position 1, the latest position.

If you want both lists to persist after restarting Vim, you need to use the
viminfo file and `:h viminfo-'`.

**NOTE**: The position before the latest jump is also kept as a [mark](#marks)
and can be jumped to via ``` `` ``` or `''`.

Help:

```
:h changelist
:h jumplist
```

## Undo tree

The latest changes to the text state are remembered. You can use _undo_ to
revert changes and _redo_ to reapply previously reverted changes.

The important bit to understand it that the data structure holding recent
changes is not a
[queue](https://en.wikipedia.org/wiki/Queue_(abstract_data_type)) but a
[tree](https://en.wikipedia.org/wiki/Tree_(data_structure))! Your changes are
nodes in the tree and each (but the top node) has a parent node. Each node keeps
information about the changed text and time. A branch is a series of nodes that
starts from any node and goes up to the top node. New branches get created when
you undo a change and then insert something else.

```
ifoo<esc>
obar<esc>
obaz<esc>
u
oquux<esc>
```

Now you have 3 lines and the undo tree looks like this:

```
     foo(1)
       /
    bar(2)
   /      \
baz(3)   quux(4)
```

The undo tree has 4 changes. The numbers represent the _time_ the nodes were
created.

Now there are two ways to traverse this tree, let's call them _branch-wise_ and
_time-wise_.

Undo (`u`) and redo (`<c-r>`) work branch-wise. They go up and down the current
branch. `u` will revert the text state to the one of node "bar". Another `u`
will revert the text state even further, to the one of node "foo". Now `<c-r>`
goes back to the state of node "bar" and another `<c-r>` to the state of node
"quux". (There's no way to reach node "baz" using branch-wise commands anymore.)

Opposed to this, `g-` and `g+` work time-wise. Thus, `g-` won't revert to the
state of node "bar", like `u` does, but to the chronologically previous state,
node "baz". Another `g-` would revert the state to the one of node "bar" and so
on. Thus, `g-` and `g+` simply go back and forth in time, respectively.

| Command / Mapping | Action |
|-------------------|--------|
| `[count]u`, `:undo [count]` | Undo [count] changes. |
| `[count]<c-r>`, `:redo` | Redo [count] changes. |
| `U` | Undo all changes to the line of the latest change. |
| `[count]g-`, `:earlier [count]?` | Go to older text state [count] times. The "?" can be either "s", "m", "h", "d", or "f". E.g. `:earlier 2d` goes to the text state from 2 days ago. `:earlier 1f` will go to the state of the latest file save. |
| `[count]g+`, `:later [count]?` | Same as above, but other direction. |

The undo tree is kept in memory and will be lost when Vim quits. See [Undo
files](#undo-files) for how to enable persistent undo.

If you're confused by the undo tree,
[undotree](https://github.com/mbbill/undotree) does a great job at visualizing
it.

Help:

```
:h undo.txt
:h usr_32
```

## Quickfix and location lists

The quickfix list is a data structure that holds file positions. Essentially,
each entry in the quickfix list consists of a file path, a line number and
optional column, and a description.

Typical use cases are assembling compiler errors or results of a grep tool.

Vim has a special type of buffer for showing the quickfix list: the quickfix
buffer. Each line in the quickfix buffer shows one entry from the quickfix list.

Usually you open a new window to display the quickfix list: the quickfix window.
When that happens, the last window gets associated with the quickfix window.

In the quickfix buffer `<cr>` opens the selected entry in the associated window
and `<c-w><cr>` in a new window.

The quickfix list was named after the "quick fix" feature from the [Aztec C
compiler](https://en.wikipedia.org/wiki/Aztec_C).

Actually there are two kinds of lists: quickfix and location lists. They behave
almost the same, but have the follwing differences:

- There is only one quickfix list. There can be multiple location lists; one per
  window.
- They use slightly different commands for navigation.

| Action         | Quickfix     | Location     |
|----------------|--------------|--------------|
| open window    | `:copen`     | `:lopen`     |
| close window   | `:cclose`    | `:lclose`    |
| next entry     | `:cnext`     | `:lnext`     |
| previous entry | `:cprevious` | `:lprevious` |
| first entry    | `:cfirst`    | `:lfirst`    |
| last entry     | `:clast`     | `:llast`     |

Mind that the quickfix and location windows don't need to be open for these
commands to work.

See `:h quickfix` for more information and a full list of commands.

For conciseness, _quickfix_ and _location_ are often abbreviated as _qf_ and
_loc_ respectively.

**Example**:

Let us use our good old friend `grep` for searching the files in the current
directory recursively for a certain query and put the results in the quickfix
list.

```vim
:let &grepprg = 'grep -Rn $* .'
:grep! foo
<grep output - hit enter>
:copen
```

Assuming any files contained the string "foo", it should be shown now in the
quickfix window.

## Macros

Vim allows _recording_ typed characters into a [register](#registers). It's a
great way to automate certain tasks on the fly. (For more elaborate tasks, Vim
scripting should be used instead.)

- Start recording by typing `q` followed by the register, e.g. `q`. (The
  command-line will signify this via "recording @q".)
- Stop recording by hitting `q` once again.
- Execute the macro via `[count]@q`.
- Repeat the last used macro via `[count]@@`.

**Example 1:**

Insert a line and repeat it 10 times:

```
qq
iabc<cr><esc>
q
10@q
```

(The same could be done without macros: `oabc<esc>10.`)

**Example 2:**

For adding line numbers in front of all lines, start on the first line and add
"1. " to it manually. Increment the number under the cursor by using `<c-a>`,
displayed as `^A`.

```
qq
0yf jP0^A
q
1000@q
```

Here we simply hope that the file doesn't contain more than 1000 lines when
using `1000@q`, but we can also use a _recursive macro_, which executes until
the macro can't be applied to a line anymore:

```
qq
0yf jP0^A@q
q
@q
```

(The same could be done without macros: `:%s/^/\=line('.') . '. '`)

Mind that I also show how to achieve the same without using macros, but this
mostly works only for such simple examples. For more complex automation, macros
are the bomb!

Also see: [Quickly edit your macros](#quickly-edit-your-macros)

Help:

```
:h recording
:h 'lazyredraw'
```

## Colorschemes

Colorschemes are the way to style your Vim. Vim consists of many components and
each of those can be customized with different colors for the foreground,
background and a few other attributes like bold text etc. They can be set like
this:

```vim
:highlight Normal ctermbg=1 guibg=red
```

This would paint the background of the editor red. See `:h :highlight` for more
information.

So, colorschemes are mostly collections of `:highlight` commands.

Actually, most colorschemes are really 2 colorschemes! The example above sets
colors via `ctermbg` and `guibg`. The former definition (`cterm*`) will only be
used if Vim was started in a terminal emulator, e.g. xterm. The latter (`gui*`)
will be used in graphical environments like gvim or MacVim.

If you ever happen to use a colorscheme in terminal Vim and the colors don't
look like the ones in the screenshot at all, chances are that the colorscheme
only defines colors for the GUI. Conversely, if you use a graphical Vim (e.g.
gvim or MacVim) and the colors look off, the colorscheme might only define
colors for the terminal.

The latter case can be "solved" by enabling true colors in Neovim or Vim
7.4.1830 and newer. This makes terminal Vim use the GUI definitions instead, but
also requires the terminal emulator itself and all software in between (e.g.
tmux) to be capable of handling true colors. ([This
gist](https://gist.github.com/XVilka/8346728) gives a good overview about the
topic.)

Help:

- `:h 'termguicolors'`
- [List of colorschemes](PLUGINS.md#colorschemes-1)
- [Cosmetic changes to colorschemes](#cosmetic-changes-to-colorschemes)

## Folding

Every text (or source code) has a certain structure. If you have a structure, it
means you have regions of logically separated text. Folding allows to "fold"
such a region into a single line and displaying a short description. There are
many commands that act on these regions called _folds_. Folds can be nested.

Vim distinguishes between several types of fold methods:

| 'foldmethod' | Usage |
|--------------|-------|
| diff         | Used in diff windows to fold unchanged text. |
| expr         | Uses `'foldexpr'` to basically create a new fold method. |
| indent       | Folds based on indentation. |
| manual       | Create folds yourself via `zf`, `zF`, and `:fold`. |
| marker       | Folds based on markers in the text (often in comments). |
| syntax       | Folds based on syntax, e.g. folding `if` blocks. |

**NOTE**: Folding can be computationally intensive! If you experience any
performance drawbacks (small delays when typing), have a look at
[FastFold](https://github.com/Konfekt/FastFold), which prevents Vim from
updating folds when it's not needed.

Help:

```
:h usr_28
:h folds
```

## Sessions

If you save a **view** (`:h :mkview`), the current state of the window (and
options and mappings) gets saved for later use (`:h :loadview`).

A **session** saves the views of all windows plus global settings. It basically
makes a snapshot of your current Vim instance and saves it in a session file.
Let me stress this: it saves the current state; everything done after saving a
session won't be part of the session file. To "update" a session, simply write
it out again.

This makes it perfect for saving your _projects_ and easy to switch between
them.

Try it right now! Open a few windows and tabs and do `:mksession Foo.vim`. If
you omit the filename, `Session.vim` will be assumed. The file will be saved to
the current working directory, check `:pwd`. Restart Vim and do `:source
Foo.vim` and voilà, the buffer list, window layout, mappings, working directory
etc. should all be the same as before you saved the session. Do some more work
and update the session by overwriting the already existing session file with
`:mksession! Foo.vim`.

Note that a session file is really just a collection of Vim commands that are
supposed to restore a certain state of a Vim instance, so feel free to take a
look at it: `:vs Foo.vim`.

You can tell Vim what things to save in a session by setting `'sessionoptions'`.

For scripting purposes Vim keeps the name of the last sourced or written session
in the internal variable `v:this_session`.

Help:

```
:h Session
:h 'sessionoptions'
:h v:this_session
```

## Locality

Many of the concepts mentioned above also have _local_ counterparts:

| Global | Local | Scope | Help |
|--------|-------|-------|------|
| `:set`     | `:setlocal`           | buffer or window | `:h local-options`    |
| `:map`     | `:map <buffer>`       | buffer           | `:h :map-local`       |
| `:autocmd` | `:autocmd * <buffer>` | buffer           | `:h autocmd-buflocal` |
| `:cd`      | `:lcd`                | window           | `:h :lcd`             |
| `<leader>` | `<localleader>`       | buffer           | `:h maplocalleader`   |

[Variables also have different scopes](https://vimhelp.appspot.com/usr_41.txt.html#41.2).

# Usage

## Nhận hỗ trợ không cần kết nối mạng

Vim comes with great documentation in the form of single text files with a
special layout. Vim uses a system based on tags for accessing certain parts of
those help files.

First of all, read this: `:help :help`. This will open the file
`$VIMRUNTIME/doc/helphelp.txt` in a new window and jump to the `:help` tag
within that file.

A few simple rules:

- options are enclosed in single quotes, e.g. `:h 'textwidth'`
- VimL functions end in `()`, e.g. `:h reverse()`
- commands start with `:`, e.g. `:h :echo`

You can use `<c-d>` (this is <kbd>ctrl</kbd>+<kbd>d</kbd>) to list all tags that
match the currently entered query. E.g. `:h tab<c-d>` will get you a list of all
tags from `tab` over `'softtabstop'` to `setting-guitablabel`.

You want to list all VimL functions? Simple: `:h ()<c-d>`. You want to list all
VimL functions that concern windows? `:h win*()<c-d>`.

This quickly becomes second nature, but especially in the beginning, you
sometimes don't know any part of the tag you are looking for. You can only
imagine some keywords that could be involved. `:helpgrep` to the rescue!

```
:helpgrep backwards
```

This will look for "backwards" in all documentation files and jump to the first
match. The matches will be assembled in the quickfix list. Use `:cn`/`:cp` to
jump to the next/previous match. Or use `:copen` to open the quickfix window,
navigate to an entry and hit `<cr>` to jump to that match. See `:h quickfix` for
the whole truth.

## Getting help offline (alternative)

This list was compiled by @chrisbra, one of the most active Vim developers, and
posted to [vim_dev](https://groups.google.com/forum/#!forum/vim_dev).

It's reposted here with minor changes.

---

If you know what you are looking for, it is usually easier to search for it
using the help system, because the subjects follow a certain style guide.

Also, the help has the advantage of belonging to your particular Vim version, so
that obsolete topics or topics that have been added later won't turn up.

Therefore, it is essential to learn the help system and the language it uses.
Here are some examples (not necessarily complete and I might have forgotten
something).

1. Options are enclosed in single quotes. So you would use `:h 'list'` to go to
   the help topic for the list option. If you only know, you are looking for a
   certain option, you can also do `:h options.txt` to open the help page which
   describes all option handling and then you can search using regular
   expressions e.g. `/width`. Certain options have their own namespace, e.g. `:h
   cpo-a`, `:h cpo-A`, `:h cpo-b`, and so on.

2. Normal mode commands are just that. Use `:h gt` to go to the help page for
   the "gt" command.

3. Regexp items always start with "/", so `:h /\+` takes you to the help item
   for the "\+" quantifier in Vim regexes. If you need to know anything about
   regular expressions, start reading at `:h pattern.txt`.

4. Key combinations. They usually start with a single letter indicating the mode
   for which they can be used. E.g. `:h i_CTRL-X` takes you to the family of
   CTRL-X commands for insert mode which can be used to auto complete different
   things. Note that certain keys will always be written the same, e.g. Control
   will always be CTRL. Note, for normal mode commands, the "n" is left away,
   e.g. `:h CTRL-A`. In contrast, `:h c_CTRL-R` will describe what CTRL-R does
   when entering commands in the command line and `:h v_Ctrl-A` talks about
   incrementing numbers in visual mode and `:h g_CTRL-A` talks about the g<C-A>
   command (thus you have to press "g" then <Ctrl-A>). Here the "g" stand for
   the normal command "g" which always expect a second key before doing
   something similar to the commands starting with "z".

5. Registers always start with "quote" so use `:h quote` to find out about the
   special ":" register.

6. Vim script (VimL) is available at `:h eval.txt`. Certain aspects of the
   language are available at `:h expr-X` where 'X' is a single letter, e.g. `:h
   expr-!` will take you to the topic describing the '!' (Not) operator for
   VimL. Also important, see `:h function-list` to find a short description of
   all functions available.

7. Mappings are talked about in the help page `:h map.txt`. Use `:h mapmode-i`
   to find out about the `:imap` command. Also use `:map-topic` to find out
   about certain subtopics particular for mappings (e.g. `:h :map-local` for
   buffer-local mappings or `:h map_bar` for how the '|' is handled in mappings.

8. Command definitions are talked about at `:h command-*`, so use :h command-bar
   to find out about the '!' argument for custom commands.

9. Window management commands always start with CTRL-W, so you find the
   corresponding help at `:h CTRL-W_*` (e.g. `:h CTRL-W_p` for switch to the
   previously accessed window). You can also access `:h windows.txt` and read
   your way through, if you are looking for window handling command.

10. Ex commands always start with ":", so `:h :s` covers the ":s" command.

11. Use CTRL-D after typing a topic and let Vim try to complete to all available
    topics.

12. Use `:helpgrep` to search in all help pages (usually also includes help
    pages by installed plugins). See `:h :helpgrep` for how to use it. Once you
    have searched for a topic, all matches are available in the quickfix (or
    location) window which can be opened with `:copen` or `:lopen`. There you
    can also use `/` to further filter the matches.

13. `:h helphelp` contains some information on how to use the help.

14. The user manual. This describes help topics for beginners in a rather
    friendly way. Start at `:h usr_toc.txt` to find the table of content (as you
    might have guessed). Skimming over that help to find certain topics, .e.g
    you will find an entry "Digraphs" and "Entering special characters" in
    chapter 24 (so use `:h usr_24.txt` to go to that particular help page).

15. Highlighting groups always start with `hl-*`. E.g. `:h hl-WarningMsg` talks
    about the "WarningMsg" highlighting group.

16. Syntax highlighting is namespaced to ":syn-topic", e.g. `:h :syn-conceal`
    talks about the conceal argument for the :syn command.

17. Quickfix commands usually start with ":c", while location list commands
    usually start with ":l".

18. `:h BufWinLeave` talks about the BufWinLeave autocmd. Also, `:h
    autocommands-events` talks about all possible events.

19. Startup arguments always start with "-", so `:h -f` takes you to the help of
    the "-f" command switch of Vim.

20. Compiled extra features always start with "+", so `:h +conceal` talks about
    the conceal support.

21. Error codes can be looked up directly in the help. `:h E297` takes you
    exactly to the description of the error message. Sometimes however, those
    error codes are not described, but rather are listed at the Vim command that
    usually causes this. E.g. `:h hE128` takes you directly to the `:function`
    command.

22. Documentation for included syntax files is usually available at `:h
    ft-*-syntax`. E.g. `:h ft-c-syntax` talks about the C syntax file and the
    options it provides. Sometimes, additional sections for omni completion (`:h
    ft-php-omni`) or filetype plugins (`:h ft-tex-plugin`) are available.

Also, a link to the user documentation (which describes certain commands more
from a user perspective and less detailed) will be mentioned at the top of help
pages if they are available. So `:h pattern.txt` mentions the user guide topics
`:h 03.9` and `:h usr_27`.

## Getting help online

If you have an issue you can't resolve or are in need of general guidance, see
the [vim_use](https://groups.google.com/forum/#!forum/vim_use) mailing list.
Another great resource is using
[IRC](https://de.wikipedia.org/wiki/Internet_Relay_Chat). The channel `#vim` on
[Freenode](https://freenode.net) is huge and usually full of helpful people.

If you want to report a Vim bug, use the
[vim_dev](https://groups.google.com/forum/#!forum/vim_dev) mailing list.

## Autocmds in practice

You can trigger any event right now: `:doautocmd BufRead`.

### User events

Especially for plugins it's useful to create your own "User" events:

```vim
function! Chibby()
  " A lot of stuff is happening here.
  " And at last..
  doautocmd User ChibbyExit
endfunction
```

Now users of your plugin can execute anything when Chibby finishes running:

```vim
autocmd User ChibbyExit call ChibbyCleanup()
```

By the way, if there's no "catching" :autocmd, :doautocmd will output a pesky
"No matching autocommands" message. That's why many plugins use `silent
doautocmd ...` instead. But this has the disadvantage, that you can't simply use
`echo "foo"` in the :autocmd, you have to use `unsilent echo "foo"` instead..

That's why it's better to check if there even is a receiving autocmd and not
bothering emitting the event otherwise:

```vim
if exists('#User#ChibbyExit')
  doautocmd User ChibbyExit
endif
```

Help: `:h User`

### Nested autocmds

By default, autocmds do not nest! If an autocmd executes a command, which in
turn would usually trigger another event, it won't happen.

Let's say every time you start Vim, you want to automatically open your vimrc:

```vim
autocmd VimEnter * edit $MYVIMRC
```

When you now start Vim, it will open your vimrc, but the first thing you'll
notice is that there won't be any highlighting although usually there would be.

The problem is that `:edit` in your non-nested autocmd won't trigger the
"BufRead" event, so the filetype never gets set to "vim" and
`$VIMRUNTIME/syntax/vim.vim` never sourced. See `:au BufRead *.vim`. Use this
instead:

```vim
autocmd VimEnter * nested edit $MYVIMRC
```

Help: `:h autocmd-nested`

## Clipboard

Required [features](#what-kind-of-vim-am-i-running): `+clipboard` and optionally
`+xterm_clipboard` if you want to use the `'clipboard'` option on a Unix system
with a Vim that doesn't have GUI support.

Help:

```
:h 'clipboard'
:h gui-clipboard
:h gui-selections
```

Also see: [Bracketed paste (or why do I have to set 'paste' all the
time?)](#bracketed-paste-or-why-do-i-have-to-set-paste-all-the-time)

### Clipboard usage (Windows, macOS)

Windows comes with a
[clipboard](https://msdn.microsoft.com/en-us/library/windows/desktop/ms649012(v=vs.85).aspx)
and macOS comes with a
[pasteboard](https://developer.apple.com/library/mac/documentation/Cocoa/Conceptual/PasteboardGuide106/Introduction/Introduction.html#//apple_ref/doc/uid/TP40008100-SW1).

Both work like most users would expect them to work. You copy selected text with
`ctrl+c`/`cmd+c` and paste them in another application with `ctrl+v`/`cmd+v`.

Note that copied text is actually transferred to the clipboard, so you can close
the application you copied from before pasting in another application without
problems.

Whenever this happens, the clipboard register `*` gets filled with the
selection. From Vim use `"*y` and `"*p` to yank and paste from the clipboard
respectively.

If you don't even want to specify the `*` register all the time, put this in
your vimrc:

```vim
set clipboard=unnamed
```

Usually all yank/delete/put operations fill the `"` register, now the `*`
register is used for the same operations, therefore simply `y` and `p` will be
enough.

Let me repeat: Using the option above means that every yank/paste, even when
only used in the same Vim window, will alter the clipboard. Decide for yourself
if this is useful or not.

If you're even too lazy to type `y`, you can send every visual selection to the
clipboard by using these settings:

```vim
set clipboard=unnamed,autoselect
set guioptions+=a
```

Help:

```
:h clipboard-unnamed
:h autoselect
:h 'go_a'
```

### Clipboard usage (Linux, BSD, ...)

If your OS uses [X](http://www.x.org/wiki), things work a bit different. X
implements the [X Window System
Protocol](http://www.x.org/releases/X11R7.7/doc/xproto/x11protocol.html) which
happens to be at major version 11 since 1987, hence X is also often called X11.

Prior, in X10, [cut
buffers](http://www.x.org/releases/X11R7.7/doc/xorg-docs/icccm/icccm.html#Peer_to_Peer_Communication_by_Means_of_Cut_Buffers)
were introduced that kind of worked like a _clipboard_ as in copied text was
actually held by X and it was accessible by all other applications. This
mechanism still exists in X, but its use is deprecated now and most software
doesn't use it anymore.

Nowadays data is transferred between applications by the means of
[selections](http://www.x.org/releases/X11R7.7/doc/xorg-docs/icccm/icccm.html#Peer_to_Peer_Communication_by_Means_of_Selections).
From the 3 _selection atoms_ defined, only 2 are used in practice: PRIMARY and
CLIPBOARD.

Selections work roughly like this:

```
Program A: <ctrl+c>
Program A: assert ownership of CLIPBOARD
Program B: <ctrl+v>
Program B: note that ownership of CLIPBOARD is hold by Program A
Program B: request data from Program A
Program A: respond to request and send data to Program B
Program B: receives data from Program A and inserts it into the window
```

| Selection | When used? | How to paste? | How to access from Vim? |
|-----------|------------|---------------|-------------------------|
| PRIMARY   | Selecting text              | `middle-click`, `shift+insert` | `*` register |
| CLIPBOARD | Selecting text and `ctrl+c` | `ctrl+v`                       | `+` register |

**NOTE**: Selections (no, not even the CLIPBOARD selection) are never kept in
the X server! Thus, you lose the data copied with `ctrl+c` when the application
closes.

Use `"*p` to paste the PRIMARY selection or `"+y1G` to yank the entire file to
the CLIPBOARD selection.

If you happen to access one of the two registers all the time, consider using:

```vim
set clipboard^=unnamed      " * register
" or
set clipboard^=unnamedplus  " + register
```

(The `^=` is used to prepend to the default value, `:h :set^=`.)

This will make all yank/delete/put operations use either `*` or `+` instead of
the unnamed register `"`. Afterwards you can simply use `y` or `p` for accessing
your chosen X selection.

Help:

```vim
:h clipboard-unnamed
:h clipboard-unnamedplus
```

## Restore cursor position when opening file

When you open a file, the cursor will be positioned at line 1, column 1.
Fortunately the viminfo file remembers [marks](#marks). The `"` mark contains
the position in the buffer where you left off.

```vim
autocmd BufReadPost *
    \ if line("'\"") > 1 && line("'\"") <= line("$") |
    \   execute "normal! g`\"" |
    \ endif
```

Read: If the mark `"` contains a line number greater than line 1 but not greater
than the last line in the file, jump to it.

    :h viminfo-'
    :h `quote
    :h g`

## Temporary files

### Backup files

Before saving a file, Vim creates a backup file. If writing to disk was
successful, the backup file will be deleted.

With `:set backup`, the backup will persist. This means, the backup file will
always have the same content as the original file _before_ the most recent save.
It's up to you to decide whether this is useful or not.

You can disable backups entirely with `:set nobackup nowritebackup`, but you
shouldn't need to nowadays. `'writebackup'` is a security feature that makes
sure that you don't lose the original file in case saving it should ever fail,
no matter whether you keep the backup file afterwards or not.

If you frequently use Vim to edit huge files, [and you probably
shouldn't](#editing-huge-files-is-slow), you can exclude those from backups with
`'backupskip'`.

Vim knows different ways to create a backup: _copying_ and _renaming_.

- **Copying**
    1. A full copy of the original file is created and used as backup.
    1. The original file gets emptied and then filled with the content of the
    Vim buffer.
- **Renaming**
    1. The original file is renamed to the backup file.
    1. The content of the Vim buffer gets written to a new file with the name of
    the original file.

See `:h 'backupcopy'` for all the nitty-gritty details.

---

Demo:

```vim
:set backup backupskip= backupdir=. backupext=-backup
:e /tmp/foo
ifoo<esc>
:w
" original file gets created, no need for backup file
obar<esc>
:w
" backup file is created, original file gets updated
```

```diff
$ diff -u /tmp/foo-backup /tmp/foo
--- /tmp/foo-backup     2017-04-22 15:05:13.000000000 +0200
+++ /tmp/foo    2017-04-22 15:05:25.000000000 +0200
@@ -1 +1,2 @@
 foo
+bar
```

---

    :h backup
    :h write-fail

### Swap files

When editing a file, unsaved changes get written to a swap file.

Get the name of the current swap file with `:swapname`. Disable them with `:set
noswapfile`.

A swap file gets updated either all 200 characters or when nothing was typed for
4 seconds. They get deleted when you stop editing the file. You can change these
numbers with `:h 'updatecount'` and `:h 'updatetime'`.

If Vim gets killed (e.g. power outage), you lose all changes since the last time
the file was written to disk, but the swap file won't be deleted. Now, if you
edit the file again, Vim will offer the chance to recover the file from the swap
file.

When two people try to edit the same file, the second person will get a notice
that the swap file already exists. It prevents people from trying to save
different versions of a file. If you don't want that behaviour, see `:h
'directory'`.

    :h swap-file
    :h usr_11

### Undo files

The [undo tree](#undo-tree) is kept in memory and will be lost when Vim quits.
If you want it to persist, `:set undofile`. This will save the undo file for
`~/foo.c` in `~/foo.c.un~`.

    :h 'undofile'
    :h undo-persistence

### Viminfo files

When backup, swap, and undo files are all about text state, viminfo files are
used for saving everything else that would otherwise be lost when quitting Vim.
The viminfo file keeps histories (command line, search, input), registers,
marks, buffer list, global variables etc.

By default, the viminfo is written to `~/.viminfo`.

    :h viminfo
    :h 'viminfo'

### Example configuration for temporary files

Put all temporary files in their own directory under `~/.vim/files`:

```vim
" create directory if needed
if !isdirectory($HOME.'/.vim/files') && exists('*mkdir')
  call mkdir($HOME.'/.vim/files')
endif

" backup files
set backup
set backupdir   =$HOME/.vim/files/backup/
set backupext   =-vimbackup
set backupskip  =
" swap files
set directory   =$HOME/.vim/files/swap//
set updatecount =100
" undo files
set undofile
set undodir     =$HOME/.vim/files/undo/
" viminfo files
set viminfo     ='100,n$HOME/.vim/files/info/viminfo
```

## Editing remote files

Vim comes with the netrw plugin that enables editing remote files. Actually it
transfers the remote file to a local temporary file via scp, opens a buffer
using that file, and writes the changes back to the remote file on saving.

This is extremely useful if you want to use your local configuration opposed to
ssh'ing into a server and use whatever the admins want you to use.

```
:e scp://bram@awesome.site.com/.vimrc
```

If you have a `~/.ssh/config` set up already, this gets used automatically:

```
Host awesome
    HostName awesome.site.com
    Port 1234
    User bram
```

Assuming the above content in `~/.ssh/config`, this works just as well:

```
:e scp://awesome/.vimrc
```

Similar can be done with a `~/.netrc`, see `:h netrw-netrc`.

Make sure to read `:h netrw-ssh-hack` and `:h g:netrw_ssh_cmd`.

---

Another possibility is using [sshfs](https://wiki.archlinux.org/index.php/Sshfs)
which uses [FUSE](https://en.wikipedia.org/wiki/Filesystem_in_Userspace) to
mount a remote filesystem into your local filesystem.

## Managing plugins

[Pathogen](https://github.com/tpope/vim-pathogen) was the first popular tool for
managing plugins. Actually it just adjusts the _runtimepath_ (`:h 'rtp'`) to
include all the things put under a certain directory. You have to clone the
repositories of the plugins there yourself.

Real plugin managers expose commands that help you to install and update plugins
from within Vim.

[List of plugin managers](PLUGINS.md#plugin-managers)

## Block insert

This is a technique to insert the same text on multiple consecutive lines at the
same time. See this
[demo](https://raw.githubusercontent.com/mhinz/vim-galore/master/static/images/content-block_insert.gif).

Switch to visual block mode with `<c-v>`. Afterwards go down for a few lines.
Hit `I` or `A` and start entering your text.

It might be a bit confusing at first, but text is always entered for the current
line and only after finishing the current insertion, the same text will be
applied to all other lines of the prior visual selection.

So a simple example is `<c-v>3jItext<esc>`.

If you have lines of different length and want to append the same text right
after the end of each line, do this: `<c-v>3j$Atext<esc>`.

Sometime you need to place the cursor somewhere after the end of the current
line. You can't do that by default, but you can set the `virtualedit` option:

```vim
set virtualedit=all
```

Afterwards `$10l` or `90|` work even after the end of the line.

See `:h blockwise-examples` for more info. It might seem complicated at first,
but quickly becomes second nature.

If you want to get real fancy, have a look at
[multiple-cursors](https://github.com/terryma/vim-multiple-cursors).

## Running external programs and using filters

Disclaimer: Vim is single-threaded, so running an external program in the
foreground will block everything else. Sure, you can use one of Vim's
programming interfaces, e.g. Lua, and use its thread support, but during that
time the Vim process is blocked nevertheless. Neovim fixed that by adding a
proper job API.

(Apparently Bram is thinking about adding job control to Vim as well. If you
have a very recent version, see `:helpgrep startjob`.)

Use `:!` to start a job. If you want to list the files in the current working
directory, use `:!ls`. Use `|` for piping in the shell as usual, e.g. `:!ls -1 |
sort | tail -n5`.

Without a range, the output of `:!` will be shown in a scrollable window. On the
other hand, if a range is given, these lines will be
[filtered](https://en.wikipedia.org/wiki/Filter_(software)). This means they
will be piped to the
[stdin](https://en.wikipedia.org/wiki/Standard_streams#Standard_input_.28stdin.29)
of the filter program and after processing be replaced by the
[stdout](https://en.wikipedia.org/wiki/Standard_streams#Standard_output_.28stdout.29)
of the filter. E.g. for prepending numbers to the next 5 lines, use this:

    :.,+4!nl -ba -w1 -s' '

Since manually adding the range is quite burdensome, Vim also provides some
helpers for convenience. As always with ranges, you can also select lines in
visual mode and then hit `:`. There's also an operator `!` that takes a motion.
E.g. `!ip!sort` will sort the lines of the current paragraph.

A good use case for filtering is the [Go programming
language](https://golang.org). The indentation is pretty opinionated, it even
comes with a filter called `gofmt` for indenting Go source code properly. So
plugins for Go often provide helper commands called `:Fmt` that basically do
`:%!gofmt`, so they indent all lines in the file.

People often use `:r !prog` to put the output of prog below the current line,
which is fine for scripts, but when doing it on the fly, I find it easier to use
`!!ls` instead, which replaces the current line.

    :h filter
    :h :read!

## Cscope

[Cscope](http://cscope.sourceforge.net/) does more things than
[ctags](http://ctags.sourceforge.net/), but only supports C (and C++ and Java to
some extent).

Whereas a tags file only knows where a symbol was defined, a cscope database
knows much more about your data:

- Where is this symbol defined?
- Where is this symbol used?
- What is this global symbol's definition?
- Where did this variable get its value?
- Where is this function in the source files?
- What functions call this function?
- What functions are called by this function?
- Where does the message "out of space" come from?
- Where is this source file in the directory structure?
- What files include this header file?

### 1. Build the database

Do this in the root of your project:

```sh
$ cscope -bqR
```

This will create 3 files: `cscope{,.in,.po}.out` in the current working
directory. Think of them as your database.

Unfortunately `cscope` only analyzes `*.[c|h|y|l]` files by default. If you want
to use cscope for a Java project instead, do this:

```sh
$ find . -name "*.java" > cscope.files
$ cscope -bq
```

### 2. Add the database

Open a connection to your freshly built database:

```vim
:cs add cscope.out
```

Verify that the connection was made:

```vim
:cs show
```

(Yes, you can add multiple connections.)

### 3. Query the database

```vim
:cs find <kind> <query>
```

E.g. `:cs find d foo` will list all functions that are called by `foo(...)`.

| Kind | Explanation |
|------|-------------|
| s    | **s**ymbol: find all references to the token        |
| g    | **g**lobal: find global definition(s) of the token  |
| c    | **c**alls: find all calls to the function           |
| t    | **t**ext: find all instances of the text            |
| e    | **e**grep: egrep search for the word                |
| f    | **f**ile: open the filename                         |
| i    | **i**ncludes: find files that include the filename  |
| d    | **d**epends: find functions called by this function |

I suggest some convenience mappings e.g.:

```vim
nnoremap <buffer> <leader>cs :cscope find s  <c-r>=expand('<cword>')<cr><cr>
nnoremap <buffer> <leader>cg :cscope find g  <c-r>=expand('<cword>')<cr><cr>
nnoremap <buffer> <leader>cc :cscope find c  <c-r>=expand('<cword>')<cr><cr>
nnoremap <buffer> <leader>ct :cscope find t  <c-r>=expand('<cword>')<cr><cr>
nnoremap <buffer> <leader>ce :cscope find e  <c-r>=expand('<cword>')<cr><cr>
nnoremap <buffer> <leader>cf :cscope find f  <c-r>=expand('<cfile>')<cr><cr>
nnoremap <buffer> <leader>ci :cscope find i ^<c-r>=expand('<cfile>')<cr>$<cr>
nnoremap <buffer> <leader>cd :cscope find d  <c-r>=expand('<cword>')<cr><cr>
```

So, when `:tag` (or `<c-]>`) jumps to a definition from the tags file, `:cstag`
does the same, but also takes connected cscope databases into account. The
option `'cscopetag'` makes `:tag` act like `:cstag` automatically. This is very
convenient if you already have tag-related mappings.

Help: `:h cscope`

## MatchIt

Since Vim is written in C, a lot of features assume C-like syntax. By default,
if your cursor is on `{` or `#endif`, you can use `%` to jump to the
corresponding `}` or `#ifdef` respectively.

Vim comes bundled with a plugin called matchit.vim which is not enabled by
default. It makes `%` also cycle through HTML tags, if/else/endif constructs in
VimL etc. and introduces a few new commands.

#### Installation for Vim 8

```vim
" vimrc
packadd! matchit
```

#### Installation for Vim 7 and older

```vim
" vimrc
runtime macros/matchit.vim
```

Since the documentation of matchit is pretty extensive, I suggest also doing the
following once:

```vim
:!mkdir -p ~/.vim/doc
:!cp $VIMRUNTIME/macros/matchit.txt ~/.vim/doc
:helptags ~/.vim/doc
```

#### Small intro

The plugin is ready to use now. See `:h matchit-intro` for the supported
commands and `:h matchit-languages` for the supported languages.

That said, it's easy to define your own matching pairs:

```vim
autocmd FileType python let b:match_words = '\<if\>:\<elif\>:\<else\>'
```

Afterwards you can cycle through these 3 statements in any Python file by using
`%` (forward) or `g%` (backward).

Help:

```
:h matchit-install
:h matchit
:h b:match_words
```

## True colors

Using true colors in a terminal emulator means being able to use 24 bits for RGB
colors. That makes 16777216 (2^24) colors instead of the usual 256.

As explained [here](#colorschemes), colorschemes can actually be _two_
colorschemes by having definitions for terminals (xterm) and for GUIs (gvim).
This made sense before terminal emulators learned about true colors.

After `:set termguicolors`, Vim starts emitting escape sequences only understood
by a terminal emulator that supports true colors. When your colors look weird,
chances are your terminal emulator doesn't support true colors or your
colorcheme has no GUI colors defined.

Many people use the terminal multiplexer
[tmux](https://github.com/tmux/tmux/wiki) which basically sits in between the
terminal emulator and Vim. To make tmux _forward_ the true color escape
sequences emitted by Vim, you have to put the following in the user's
`.tmux.conf`:

```
set-option -g  default-terminal 'tmux-256color'
set-option -ga terminal-overrides ',xterm-256color:Tc'
```

- The first line should be the same for most people and denotes the `$TERM` to
  be used _within_ tmux.
- The second line adds the tmux-specific `Tc` (true color) capability to the
  other terminfo entries of `xterm-256color`. Obviously this assumes that the
  user is using `TERM=xterm-256color` _outside_ of tmux.

So, here is the checklist for enabling true colors:

- Read `:h 'termguicolors'`.
- Put `set termguicolors` in your vimrc.
- Make sure your colorscheme has color definitions for GUIs. (It should contain
  lines with `guifg` and `guibg`.)
- Make sure your terminal emulator of choice supports true colors.
- Using tmux? Configure it to add the `Tc` capability.

A popular reference for colors in the terminal:
https://gist.github.com/XVilka/8346728

# Tips

## Go to other end of selected text

`o` and `O` in a visual selection make the cursor go to the other end. Try with
blockwise selection to see the difference. This is useful for quickly changing
the size of the selected text.

```
:h v_o
:h v_O
```

## Saner behavior of n and N

The direction of `n` and `N` depends on whether `/` or `?` was used for
searching forward or backward respectively. This is pretty confusing to me.

If you want `n` to always search forward and `N` backward, use this:

```vim
nnoremap <expr> n  'Nn'[v:searchforward]
xnoremap <expr> n  'Nn'[v:searchforward]
onoremap <expr> n  'Nn'[v:searchforward]

nnoremap <expr> N  'nN'[v:searchforward]
xnoremap <expr> N  'nN'[v:searchforward]
onoremap <expr> N  'nN'[v:searchforward]
```

## Saner command-line history

If you're anything like me, you're used to going to next and previous items via
`<c-n>` and `<c-p>` respectively. By default, this also works in the
command-line and recalls older or more recent command-lines from history.

So far, so good. But `<up>` and `<down>` are even smarter! They recall the
command-line whose beginning matches the current command-line. E.g. `:echo <up>`
may change to `:echo "Vim rocks!"`.

Of course, I don't want you to reach to the arrow keys, just map it instead:

```vim
cnoremap <c-n>  <down>
cnoremap <c-p>  <up>
```

I depend on this behaviour several times a day.

## Saner CTRL-L

By default, `<c-l>` clears and redraws the screen (like `:redraw!`). The
following mapping does the same, plus de-highlighting the matches found via `/`,
`?` etc., plus fixing syntax highlighting (sometimes Vim loses highlighting due
to complex highlighting rules), plus force updating the syntax highlighting in
diff mode:

```vim
nnoremap <leader>l :nohlsearch<cr>:diffupdate<cr>:syntax sync fromstart<cr><c-l>
```

## Disable audible and visual bells

```vim
set noerrorbells
set novisualbell
set t_vb=
```

See [Vim Wiki: Disable beeping](http://vim.wikia.com/wiki/Disable_beeping).

## Quickly move current line

Sometimes I need a quick way to move the current line above or below:

```vim
nnoremap [e  :<c-u>execute 'move -1-'. v:count1<cr>
nnoremap ]e  :<c-u>execute 'move +'. v:count1<cr>
```

These mappings also take a count, so `2]e` moves the current line 2 lines below.

## Quickly add empty lines

```vim
nnoremap [<space>  :<c-u>put! =repeat(nr2char(10), v:count1)<cr>'[
nnoremap ]<space>  :<c-u>put =repeat(nr2char(10), v:count1)<cr>
```

Now `5[<space>` inserts 5 blank lines above the current line.

## Quickly edit your macros

This is a real gem! The mapping takes a register (or `*` by default) and opens
it in the cmdline-window. Hit `<cr>` when you're done editing for setting the
register.

I often use this to correct typos I did while recording a macro.

```vim
nnoremap <leader>m  :<c-u><c-r><c-r>='let @'. v:register .' = '. string(getreg(v:register))<cr><c-f><left>
```

Use it like this `<leader>m` or `"q<leader>m`.

Notice the use of `<c-r><c-r>` to make sure that the `<c-r>` is inserted
literally. See `:h c_^R^R`.

## Quickly jump to header or source file

This technique can probably be applied to many filetypes. It sets _file marks_
(see `:h marks`) when leaving a source or header file, so you can quickly jump
back to the last accessed one by using `'C` or `'H` (see `:h 'A`).

```vim
autocmd BufLeave *.{c,cpp} mark C
autocmd BufLeave *.h       mark H
```

**NOTE**: The info is saved in the viminfo file, so make sure that `:set
viminfo?` includes `:h viminfo-'`.

## Quickly change font size in GUI

I think this was taken from tpope's config:

```vim
command! Bigger  :let &guifont = substitute(&guifont, '\d\+$', '\=submatch(0)+1', '')
command! Smaller :let &guifont = substitute(&guifont, '\d\+$', '\=submatch(0)-1', '')
```

## Change cursor style dependent on mode

I like to use a block cursor in normal mode, i-beam cursor in insert mode, and
underline cursor in replace mode.

```vim
if empty($TMUX)
  let &t_SI = "\<Esc>]50;CursorShape=1\x7"
  let &t_EI = "\<Esc>]50;CursorShape=0\x7"
  let &t_SR = "\<Esc>]50;CursorShape=2\x7"
else
  let &t_SI = "\<Esc>Ptmux;\<Esc>\<Esc>]50;CursorShape=1\x7\<Esc>\\"
  let &t_EI = "\<Esc>Ptmux;\<Esc>\<Esc>]50;CursorShape=0\x7\<Esc>\\"
  let &t_SR = "\<Esc>Ptmux;\<Esc>\<Esc>]50;CursorShape=2\x7\<Esc>\\"
endif
```

This simply tells Vim to print a certain sequence of characters ([escape
sequence](https://en.wikipedia.org/wiki/Escape_sequence)) when entering/leaving
insert mode. The underlying terminal, or programs like
[tmux](https://tmux.github.io) that sit between Vim and the terminal, will
process and evaluate it.

There's one drawback though: there are many terminal emulator implementations
and not all use the same sequences for doing the same things. The sequences used
above might not work with your implementation. Your implementation might not
even support different cursor styles. Check the documentation.

The example above works with iTerm2.

## Don't lose selection when shifting sidewards

If you select one or more lines, you can use `<` and `>` for shifting them
sidewards. Unfortunately you immediately lose the selection afterwards.

You can use `gv` to reselect the last selection (see `:h gv`), thus you can work
around it like this:

```vim
xnoremap <  <gv
xnoremap >  >gv
```

Now you can use `>>>>>` on your visual selection without any problems.

**NOTE**: The same can be achieved using `.`, which repeats the last change.

## Reload a file on saving

Using [autocmds](#autocmds) you can do anything on saving a file, e.g. sourcing
it in case of a dotfile or running a linter to check for syntactical errors in
your source code.

```vim
autocmd BufWritePost $MYVIMRC source $MYVIMRC
autocmd BufWritePost ~/.Xdefaults call system('xrdb ~/.Xdefaults')
```

## Smarter cursorline

I love the cursorline, but I only want to use it in the current window and not
when being in insert mode:

```vim
autocmd InsertLeave,WinEnter * set cursorline
autocmd InsertEnter,WinLeave * set nocursorline
```

## Faster keyword completion

The keyword completion (`<c-n>`/`<c-p>`) tries completing whatever is listed in
the `'complete'` option. By default, this also includes tags (which can be
annoying) and scanning all included files (which can be very slow). If you can
live without these things, disable them:

```vim
set complete-=i   " disable scanning included files
set complete-=t   " disable searching tags
```

## Cosmetic changes to colorschemes

Always use a dark gray statusline, no matter what colorscheme is chosen:

```vim
autocmd ColorScheme * highlight StatusLine ctermbg=darkgray cterm=NONE guibg=darkgray gui=NONE
```

This triggers every time you use `:colorscheme ...`. If you want it to trigger
only for a certain colorscheme:

```vim
autocmd ColorScheme desert highlight StatusLine ctermbg=darkgray cterm=NONE guibg=darkgray gui=NONE
```

This triggers only for `:colorscheme desert`.

# Commands

Useful commands that are good to know. Use `:h :<command name>` to learn more
about them, e.g. `:h :global`.

## :global and :vglobal

Execute a command on all matching lines. E.g. `:global /regexp/ print` will use
`:print` on all lines that contain "regexp".

Fun fact: You probably all know good old grep, the filter program written by Ken
Thompson. What does it do? It prints all lines matching a certain regular
expression! Now guess the short form of `:global /regexp/ print`? That's right!
It's `:g/re/p`. Ken Thompson was inspired by vi's `:global` when he wrote grep.

Despite its name, `:global` only acts on all lines by default, but it also takes
a range. Assume you want use `:delete` on all lines from the current line to the
next blank line (matched by the regular expression `^$`) that contain "foo":

```vim
:,/^$/g/foo/d
```

For executing commands on all lines that do _not_ match a given pattern, use
`:global!` or its alias `:vglobal` (think _inVerse_) instead.

## :normal and :execute

These commands are commonly used in Vim scripts.

With `:normal` you can do normal mode mappings from the command-line. E.g.
`:normal! 4j` will make the cursor go down 4 lines (without using any custom
mapping for "j" due to the "!").

Mind that `:normal` also takes a [range](#ranges), so `:%norm! Iabc` would
prepend "abc" to every line.

With `:execute` you can mix commands with expressions. Assume you edit a C
source file and want to switch to its header file:

```vim
:execute 'edit' fnamemodify(expand('%'), ':r') . '.h'
```

Both commands are often used together. Assume you want to make the cursor go
down "n" lines:

```vim
:let n = 4
:execute 'normal!' n . 'j'
```

## :redir and execute()

Many commands print messages and `:redir` allows to redirect that output. You
can redirect to files, [registers](#registers) or variables.

```vim
:redir => var
:reg
:redir END
:echo var
:" For fun let's also put it onto the current buffer.
:put =var
```

In Vim 8 there is an even shorter way:

```vim
:put =execute('reg')
```

Help:

```
:h :redir
:h execute()
```

# Debugging

## General tips

If you encounter a strange behaviour, try reproducing it like this:

```
vim -u NONE -N
```

This will start Vim without vimrc (thus default settings) and in nocompatible
mode (which makes it use Vim defaults instead of vi defaults). (See `:h
--noplugin` for other combinations of what to load at start.)

If you can still reproduce it now, it's most likely a bug in Vim itself! Report
it to the [vim_dev](https://groups.google.com/forum/#!forum/vim_dev) mailing
list. Most of the time the issue won't be resolved at this time and you'll have
to further investigate.

Plugins often introduce new/changed/faulty behaviour. E.g. if it happens on
saving, check `:verb au BufWritePost` to get a list of potential culprits.

If you're using a plugin manager, comment them out until you find the culprit.

Issue is still not resolved? If it's not a plugin, it must be your other
settings, so maybe your options or autocmds etc.

Time to use binary search. Repeatedly split the search space in two until you
find the culprit line. Due to the nature of binary division, it won't take many
steps.

In practice, it works like this: Put the `:finish` command in the middle of your
vimrc. Vim will skip everything after it. If it still happens, the problem is in
the active upper half. Move the `:finish` to the middle of _that_ half.
Otherwise, the issue is in the inactive lower half. Move the `:finish` to the
middle of _that_ half. And so on.

## Verbosity

Another useful way for observing what Vim is currently doing is increasing the
verbosity level. Currently Vim supports 9 different levels. See `:h 'verbose'`
for the full list.

```vim
:e /tmp/foo
:set verbose=2
:w
:set verbose=0
```

This would show all the files that get sourced, e.g. the undo file or various
plugins that act on saving.

If you only want increase verbosity for a single command, there's also
`:verbose`, which simply gets put in front of any other command. It takes the
verbosity level as count and defaults to 1:

```vim
:verb set verbose
"  verbose=1
:10verb set verbose
"  verbose=10
```

It's very often used with its default verbosity level 1 to show where an option
was set last:

```vim
:verb set ai?
"      Last set from ~/.vim/vimrc
```

Naturally, the higher the verbosity level the more overwhelming the output. But
fear no more, you can simply redirect the output to a file:

```vim
:set verbosefile=/tmp/foo | 15verbose echo "foo" | vsplit /tmp/foo
```

You can also enable verbosity at starting time, with the `-V` option. It
defaults to verbosity level 10. E.g. `vim -V5`.

## Profiling startup time

Vim startup feels slow? Time to crunch some numbers:

```
vim --startuptime /tmp/startup.log +q && vim /tmp/startup.log
```

The first column is the most important as it shows the elapsed absolute time. If
there is a big jump in time between two lines, the second line is either a very
big file or a file with faulty VimL code that is worth investigating.

## Profiling at runtime

Required [feature](#what-kind-of-vim-am-i-running): `+profile`

Vim provides a built-in capability for profiling at runtime and is a great way
to find slow code in your environment.

The `:profile` command takes a bunch of sub-commands for specifying what to
profile.

If you want to profile _everything_, do this:

    :profile start /tmp/profile.log
    :profile file *
    :profile func *
    <do something in Vim>
    :qa

Vim keeps the profiling information in memory and only writes it out to the
logfile on exit. (Neovim has fixed this using `:profile dump`).

Have a look at `/tmp/profile.log`. All code that was executed during profiling
will be shown. Every line, how often it was executed and how much time it took.

Jump to the bottom of the log. Here are two different sections `FUNCTIONS SORTED
ON TOTAL TIME` and `FUNCTIONS SORTED ON SELF TIME` that are worth gold. At a
quick glance you can see which functions are taking the longest.

You can use `:profile` during startup as well:

    $ vim --cmd 'prof start prof.log | prof file * | prof func *' test.c
    :q
    $ tail -50 prof.log

## Debugging Vim scripts

If you ever used a command-line debugger before, `:debug` will quickly feel
familiar.

Simply prepend `:debug` to any other command and you'll be put into debug mode.
That is, the execution will stop at the first line about to be executed and that
line will be displayed.

See `:h >cont` and below for the 6 available debugger commands and note that,
like in gdb and similar debuggers, you can also use their short forms: `c`, `q`,
`n`, `s`, `i`, and `f`.

Apart from that those, you're free to use any Vim command, e.g. `:echo myvar`,
which gets executed in the context of the current position in the code.

You basically get a
[REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop) by
simply using `:debug 1`.

It would be a pain if you had to single-step through every single line, so of
course we can define breakpoints, too. (Breakpoints are called breakpoints,
because the execution stops when they're hit, thus you can simply skip code
you're not interested in.) See `:h :breakadd`, `:h :breakdel`, and `:h
:breaklist` for further details.

Let's assume you want to know what code is run every time you save a file:

```vim
:au BufWritePost
" signify  BufWritePost
"     *         call sy#start()
:breakadd func *start
:w
" Breakpoint in "sy#start" line 1
" Entering Debug mode.  Type "cont" to continue.
" function sy#start
" line 1: if g:signify_locked
>s
" function sy#start
" line 3: endif
>
" function sy#start
" line 5: let sy_path = resolve(expand('%:p'))
>q
:breakdel *
```

As you can see, using `<cr>` will repeat the previous debugger command, `s` in
this case.

`:debug` can be used in combination with the [verbose](#verbosity) option.

## Debugging syntax files

Syntax files are often the cause for slowdowns due to wrong and/or complex
regular expressions. If the `+profile` [feature](#what-kind-of-vim-am-i-running)
is compiled in, Vim provides the super useful `:syntime` command.

```vim
:syntime on
" hit <c-l> a few times to redraw the window which causes the syntax rules to get applied again
:syntime off
:syntime report
```

The output contains important metrics. E.g. you can see which regexp takes too
long and should be optimized or which regexps are used all the time but never
even match.

See `:h :syntime`.

# Miscellaneous

## Additional resources

| Resource | Description |
|----------|-------------|
| [Seven habits of effective text editing](http://www.moolenaar.net/habits.html) | By Bram Moolenaar, the author of Vim. |
| [Seven habits of effective text editing 2.0 (PDF)](http://www.moolenaar.net/habits_2007.pdf) | See above. |
| [IBM DeveloperWorks: Scripting the Vim editor](http://www.ibm.com/developerworks/views/linux/libraryview.jsp?sort_order=asc&sort_by=Title&search_by=scripting+the+vim+editor) | Five-part series on Vim scripting. |
| [Learn Vimscript the Hard Way](http://learnvimscriptthehardway.stevelosh.com) | Develop a Vim plugin from scratch. |
| [Practical Vim (2nd Edition)](http://www.amazon.com/Practical-Vim-Edit-Speed-Thought/dp/1680501275/) | Hands down the best book about Vim. |
| [Why, oh WHY, do those #?@! nutheads use vi?](http://www.viemu.com/a-why-vi-vim.html) | Common misconceptions explained. |
| [Your problem with Vim is that you don't grok vi](http://stackoverflow.com/a/1220118) | Concise, informative and correct. A real gem. |

#### Screencasts

- [vimcasts.org](http://vimcasts.org/episodes/archive)
- [By wincent](https://www.youtube.com/channel/UCXPHFM88IlFn68OmLwtPmZA)
- [By Derek Wyatt](http://derekwyatt.org/vim/tutorials/index.html)

## Vim distributions

Vim distributions are bundles of custom settings and plugins for Vim.

More advanced users know how to configure their editor anyway, so distributions
are mostly targeted at beginners. If you think about that, it's quite
paradoxical though: Making it easier by adding even more things to learn about?

I know that many people don't want to spend hours and hours on customizing an
editor (and actually you never stop customizing your vimrc when you finally got
hooked), but eventually you only get efficient in Vim when you take the time to
learn it properly.

Repeat after me: "A programmer should know their tools."

Anyway, if you know what you're doing, you might draw some inspiration from
looking at a few distributions:

- [cream](http://cream.sourceforge.net)
- [janus](https://github.com/carlhuda/janus.git)
- [spacevim](https://github.com/SpaceVim/SpaceVim)
- [spf13](https://github.com/spf13/spf13-vim)

## Standard plugins

Many people are surprised by the fact that Vim comes with a handful of standard
plugins. Some get loaded by default (`:e $VIMRUNTIME/plugin`) and some are not
(`:e $VIMRUNTIME/pack/dist/opt`). Read `:h pack-add` on how to source the
latter.

Most of the plugins that get loaded by default will never get used, though.
Disable them as you see fit. They will still be shown as sourced
(`:scriptnames`), but only the first lines actually get read before Vim bails
out. No further code (mappings, commands, logic) will be processed.

| Plugin     | Disable it using..                  | Help |
|------------|-------------------------------------|------|
| 2html      | `let g:loaded_2html_plugin = 1`     | `:h 2html` |
| getscript  | `let g:loaded_getscriptPlugin = 1`  | `:h pi_getscript` |
| gzip       | `let g:loaded_gzip = 1`             | `:h pi_gzip` |
| logipat    | `let g:loaded_logipat = 1`          | `:h pi_logipat` |
| matchparen | `let g:loaded_matchparen = 1`       | `:h pi_paren` |
| netrw      | `let g:loaded_netrwPlugin = 1`      | `:h pi_netrw` |
| rrhelper   | `let g:loaded_rrhelper = 1`         | `:e $VIMRUNTIME/plugin/rrhelper.vim` |
| spellfile  | `let g:loaded_spellfile_plugin = 1` | `:h spellfile.vim` |
| tar        | `let g:loaded_tarPlugin = 1`        | `:h pi_tar` |
| vimball    | `let g:loaded_vimballPlugin = 1`    | `:h pi_vimball` |
| zip        | `let g:loaded_zipPlugin = 1`        | `:h pi_zip` |

## Map CapsLock to Control

CapsLock belongs to the most useless keys on your keyboard, but it's much easier
to reach than the Control key, since it lies on your [home
row](https://raw.githubusercontent.com/mhinz/vim-galore/master/static/images/content-homerow.png).
Mapping CapsLock to Control is a great way to prevent or at least reduce
[RSI](https://de.wikipedia.org/wiki/Repetitive-Strain-Injury-Syndrom) if you
program a lot.

Attention: When you get used to it, you can't live without it anymore.

**macOS**:

`System Preferences -> Keyboard -> Keyboard Tab -> Modifier Keys`. Change
"CapsLock" to "Control".

**Linux**:

To change the keys in X, put this in your `~/.xmodmap`:

    remove Lock = Caps_Lock
    keysym Caps_Lock = Control_L
    add Control = Control_L

Afterwards source it via `$ xmodmap ~/.xmodmap`.

An alternative would be using [caps2esc](https://github.com/oblitum/caps2esc) or
[xcape](https://github.com/alols/xcape).

**Windows**:

See [superuser.com: Map Caps-Lock to Control in Windows
8.1](http://superuser.com/questions/764782/map-caps-lock-to-control-in-windows-8-1).

## Generating HTML from buffer

Generate HTML from any buffer using `:TOhtml` from the 2html [standard
plugin](#standard-plugins). The output can be used for printing or easy web
publishing.

The command creates a new buffer of the same name with `.html` appended. The
colors are the same as seen in Vim. They depend on the
[colorscheme](#colorschemes).

The plugin knows several options to finetune the output, e.g. for setting the
encoding and font.

See `:h :TOhtml`.

## Easter eggs

| Command   | Message |
|-----------|---------|
| `:Ni!` | `Do you demand a shrubbery?` |
| `:h 'sm'` | `NOTE: Use of the short form is rated PG.` |
| `:h 42` | `What is the meaning of life, the universe and everything? Douglas Adams, the only person who knew what this question really was about is now dead, unfortunately.  So now you might wonder what the meaning of death is...` |
| `:h UserGettingBored` | `When the user presses the same key 42 times. Just kidding! :-)` |
| `:h bar` | `Ceci n'est pas une pipe.` |
| `:h holy-grail` | `You found it, Arthur!` |
| `:h map-modes` | `:nunmap can also be used outside of a monastery.` |
| `:help!` | `E478: Don't panic!` (Glitch? When used in a help buffer (`buftype=help`) this works like `:h help.txt` instead.) |
| `:smile` | Try it out yourself. ;-) Added in 7.4.1005. |

## Why hjkl for navigation?

When [Bill Joy](https://en.wikipedia.org/wiki/Bill_Joy) created
[vi](https://en.wikipedia.org/wiki/Vi), a predecessor of Vim, he did it on a
[ADM-3A](https://en.wikipedia.org/wiki/ADM-3A) which had no extra cursor buttons
but used, you might already guessed it, hjkl instead.

Keyboard layout: [click](https://raw.githubusercontent.com/mhinz/vim-galore/master/static/images/content-adm-3a-layout.jpg)

This also shows why `~` is used to denote the home directory on Unix systems.

# Common problems

## Editing small files is slow

There are two things which can have a huge impact on performance:

1. Complex **regular expressions**. Particular the Ruby syntax file caused
   people to have slowdowns in the past. (Also see [Debugging syntax files](#debugging-syntax-files).)
2. **Screen redraws**. Some features force all lines to redraw.

| Typical culprit | Why? | Solution? |
|-----------------|------|-----------|
| `:set cursorline`        | Causes all lines to redraw. | `:set nocursorline` |
| `:set cursorcolumn`      | Causes all lines to redraw. | `:set nocursorcolumn` |
| `:set relativenumber`    | Causes all lines to redraw. | `:set norelativenumber` |
| `:set foldmethod=syntax` | If the syntax file is slow already, this makes it even worse. | `:set foldmethod=manual`, `:set foldmethod=marker` or [FastFold](https://github.com/Konfekt/FastFold) |
| `:set synmaxcol=3000`    | Due to internal representation, Vim has problems with long lines in general. Highlights columns till column 3000. | `:set synmaxcol=200` |
| matchparen.vim           | Loaded by default. Uses regular expressions to find the accompanying parenthesis. | Disable plugin: `:h matchparen` |

**NOTE**: You only need to do this if you experience actual performance
drawbacks. In most cases using the things mentioned above is absolutely fine.

## Editing huge files is slow

The biggest issue with big files is, that Vim reads the whole file at once. This
is done due to how buffers are represented internally.
([Discussion on vim_dev@](https://groups.google.com/forum/#!topic/vim_dev/oY3i8rqYGD4/discussion))

If you only want to read, `tail hugefile | vim -` is a good workaround.

If you can live without syntax, settings and plugins for the moment:

```
$ vim -u NONE -N
```

This should make navigation quite a lot faster, especially since no expensive
regular expressions for syntax highlighting are used. You should also tell Vim
not to use swapfiles and viminfo files to avoid long delays on writing:

```
$ vim -n -u NONE -i NONE -N
```

Putting it in a nutshell, try to avoid using Vim when intending to write really
huge files. :\

## Bracketed paste (or why do I have to set 'paste' all the time?)

Bracketed paste mode allows terminal emulators to distinguish between typed text
and pasted text.

Did you ever tried pasting code into Vim and afterwards everything seemed messed
up?

This only happens if you paste via `cmd+v`, `shift-insert`, `middle-click` etc.
because then you're just throwing text at the terminal emulator. Vim doesn't
know that you just pasted the text, it thinks you're an extremely fast typist.
Accordingly, it tries to indent the lines and fails.

Obviously this is not an issue, if you paste using Vim's registers, e.g. `"+p`,
because then Vim knows that you're actually pasting.

To workaround this, you have to `:set paste`, so it gets pasted as-is. See `:h
'paste'` and `:h 'pastetoggle'`.

If you're fed up with toggling `'paste'` all the time, have a look at this fine
plugin that does it for you:
[bracketed-paste](https://github.com/ConradIrwin/vim-bracketed-paste).

Additional read from the same author as the plugin:
[here](http://cirw.in/blog/bracketed-paste).

**Neovim**: Neovim tries to make all of this much more seamless and sets
bracketed paste mode automatically if the terminal emulator supports it.

## Delays when using escape key in terminal

If you live in the command-line, you probably use a so-called _terminal
emulator_ like xterm, gnome-terminal, iTerm2, etc. (opposed to a real
[terminal](https://en.wikipedia.org/wiki/Computer_terminal)).

Like their ancestors, terminal emulators use [escape
sequences](https://en.wikipedia.org/wiki/Escape_sequence) (or _control
sequences_) to control things like moving the cursor, changing text colors, etc.
They're simply strings of ASCII characters starting with an escape character
(displayed in [caret notation](https://en.wikipedia.org/wiki/Caret_notation) as
`^[`). When such a string arrives, the terminal emulator looks up the
accompanying action in the [terminfo](https://en.wikipedia.org/wiki/Terminfo)
database.

To make the problem clearer, I'll explain mapping timeouts first. They always
happen when there's ambiguity between mappings:

```vim
:nnoremap ,a  :echo 'foo'<cr>
:nnoremap ,ab :echo 'bar'<cr>
```

Both mappings work as expected, but when typing `,a`, there will be a delay of 1
second, because Vim waits whether the user keys in another `b` or not.

Escape sequences pose the same problem:

- `<esc>` is used a lot for returning to normal mode or quitting an action.
- Cursor keys are encoded using escape sequences.
- Vim expects <kbd>Alt</kbd> (also called _Meta key_) to send a proper 8-bit
  encoding with the high bit set, but many terminal emulators don't support it
  (or don't enable it by default) and send an escape sequence instead.

You can test the above like this: `vim -u NONE -N` and type `i<c-v><left>` and
you'll see a sequence inserted that starts with `^[` which denotes the escape
character.

Putting it in a nutshell, Vim has a hard time distinguishing between a typed
`<esc>` character and a proper escape sequence.

By default, Vim uses `:set timeout timeoutlen=1000`, so it delays on ambiguity
of mappings _and_ key codes by 1 second. This is a sane value for mappings, but
you can define the key code timeout on its own which is the most common
workaround for this entire issue:

```vim
set timeout           " for mappings
set timeoutlen=1000   " default value
set ttimeout          " for key codes
set ttimeoutlen=10    " unnoticeable small value
```

Under `:h ttimeout` you find a small table showing the relationship between
these options.

If you're using tmux between Vim and your terminal emulator, also put this in
your `~/.tmux.conf`:

```tmux
set -sg escape-time 0
```

## Function search undo

- A search pattern in a command (`/`, `:substitute`, ...) changes the "last used
  search pattern". (It's saved in the `/` register; print it with `:echo @/`).
- A simple text change can be redone with `.`. (It's saved in the `.` register;
  print it with `:echo @.`).

Both things are _not_ the case, if you do them from a function, though! Thus you
can't easily highlight words from a function or redo the text changes made by
it.

Help: `:h function-search-undo`

# Technical quirks

## Newline used for NUL

NUL characters (`\0`) in a file, are stored as newline (`\n`) in memory and
displayed in a buffer as `^@`.

See `man 7 ascii` and `:h NL-used-for-Nul` for more information.

# Terminology

## Vim script? Vimscript? VimL?

`Vim script`, `Vimscript`, and `VimL` all refer to the same thing: The
programming language used for scripting Vim. Even though
[8.0.360](https://github.com/vim/vim/commit/b544f3c81f1e6a50322855681ac266ffaa8e313c)
changed all references to `VimL` to `Vim script`, which can now be considered
the official term, `VimL` is still widespread all over the internet.

No matter which term you use, everyone will understand it.
