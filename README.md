### will_paginate
---
https://github.com/mislav/will_paginate

```sh
gem 'will_paginate', '~> 3.1.0'
```

```ruby
@post = Post.paginate(:page => params[:page])
Post.paginate(:page => params[:page], :per_page => 30)
<%= will_paginate @posts %>


class Post
  self.per_page = 10
end
WillPaginate.per_page = 10


Post.where(:published => true).order(:page => params[:page]).order('id DESC')
Post.page(params[:page]).order('created_at DESC')

```

https://github.com/mislav/will_paginate/wiki/Installation

