# Rails Snippet v0.4.0

|Prefix|shortcut||
|---|---|---|
|pre||<%  %>|
|preb||<%  %><br><br><% end %>|
|pre-||<%=  %>|
|preb-||<%=  %><br><br><% end %>|
|each||<% @variable.each do \|variable\| %><br><br><% end %>|
|form_for||<%= form_for variable do \|f\| %><br><br><% end %>|
|simple_form_for||<%= simple_form_for variable do \|f\| %><br><br><% end %>|
|time_zone_select||<%= f.time_zone_select :id_name %>|
|range_field||<%= range_field (:model_name, :id_name, in: 1..100) %>|
|select_tag||<%= select_tag (:id_name, options_for_select(options)) %>|
|options_for_select||options_for_select([options])|
|color_field||<%= color_field :id_name %>|
|render||<%= render  \"path\" %>|
|render_variable||<%= render  "path", variable: variable %>|
|link_to||<%= link_to  \"text\", path %>|
|link_to_class|litoc|<%= link_to  "text", path, class:"class" %>|
|link_to_method_data|ltmd|<%= link_to "link_text", path, method: "method", data:{ data } %>|
|link_to_method_data|ltmdc|<%= link_to "link_text", path, method: "method", data:{ data }, class:"class" %>|
|link_to_method_confirm|ltmdc|<%= link_to "link_text", path, method: "method", data:{ confirm: "confirm" } %>|
|link_to_method_confirm_class|ltmdcc|<%= link_to "link_text", path, method: "method", data:{ confirm: "confirm" }, class:"class" %>|
|f.number_field||<%= f.number_field (:id_name, in: 1.0..20.0, step: 0.5) %>|
|f.time_field||<%= f.time_field :id_name %>|
|f.hidden_field||<%= f.hidden_field :id_name %>|
|f.email_field||<%= f.email_field :id_name %>|
|f.url_field||<%= f.url_field :id_name %>|
|f.password_field||<%= f.password_field :id_name %>|
|f.text_area||<%= f.text_area :id_name %>|
|f.check_box||<%= f.check_box :id_name %>|
|f.text_field||<%= f.text_field :id_name %>|
|f.radio_button||<%= f.radio_button :name, :value => \"value\" %>|
|f.label||<%= f.label :id_name, "text" %>|
|f.input||<%= f.input :id, label: "text" %>|
|f.submit||<%= f.submit %>|
|path||{path}_path|
|new_path||new_{path}_path|
|edit_path||edit_{path}_path|
|f.date||<%= f.date_field :id_name %>|
|f.datetime||<%= f.datetime_field :id_name %>|
|2018-1-5|||
|if||<% if $1 %><br>&nbsp;&nbsp;$2<br><% end %>|
|if else||<% if $1 %><br>&nbsp;&nbsp;$2<br><% else %><br>&nbsp;&nbsp;$3<br><% end %>|
|if elsif||<% if $1 %><br>&nbsp;&nbsp;$2<br><% elsif $3 %><br>&nbsp;&nbsp;$4<br><% end %>|
|if elsif else||<% if $1 %><br>&nbsp;&nbsp;$2<br><% elsif $3 %><br>&nbsp;&nbsp;$4<br><% else %><br>&nbsp;&nbsp;$5<br><% end %>|
|***Feature***|||

# Ruby Snippet v0.4.0


|Prefix||
|---|---|
|only|only: [:id]|
|except|except: [:id]|
## Route
|Prefix||
|---|---|
|get|get "/$1", to: "$2"|
|post|post "/$1", to: "$2"|
|patch|patch "/$1", to: "$2"|
|put|put "/$1", to: "$2"|
|delete|delete "/$1", to: "$2"|
|res|resources :res_name|
|res_block|resources :res_name do<br>  <br>end|
|res_collection_block|resources :res_name do<br>&nbsp;&nbsp;collection do<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;end<br>end|
|res_member_block|resources :res_name do<br>&nbsp;&nbsp;member do<br><br>&nbsp;&nbsp;end<br>end|
|re|resource :res_name|
|re_block|resource :res_name do<br>  <br>end|
|re_collection_block|resource :res_name do<br>&nbsp;&nbsp;collection do<br>&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;end<br>end|
|re_member_block|resource :res_name do<br>&nbsp;&nbsp;member do<br><br>&nbsp;&nbsp;end<br>end|
|member_block|member do<br><br>end<br>|
|collection_block|collection do<br><br>end|


## Redirect
|Prefix||
|---|---|
|render|render path|
|redirect_to|redirect_to path|
|redirect_to_msg|redirect_to path, notice: "msg"|

## Model
|Prefix|shortcut||
|---|---|---|
|***relationship***|||
|has_one||has_one :|
|dependent||dependent: :id|
|has_one_dependent||has_one :id, dependent: :type|
|has_many||has_many :|
|has_many_through||has_many :model1, through: :model2|
|has_many_dependent||has_many :id, dependent: :type|
|belongs_to||belongs_to :|
|belongs_to_cache||belongs_to :id, cache: true|
|has_and_belongs_to_many|habtm|has_and_belongs_to_many :id|
|***column***|||
|t.binary|tcbi|t.binary :|
|t.boolean|tcb|t.boolean :|
|t.date|tcda|t.date :|
|t.datetime|tcdt|t.datetime :|
|t.decimal|tcd|t.decimal :|
|t.float|tcf|t.float :|
|t.integer|tci|t.integer :|
|t.references|tcr|t.references :|
|t.string|tcs|t.string :|
|t.text|tct|t.text :|
|t.time|tcti|t.time :|
|t.timestamp|tcts|t.timestamp :|
|t.timestamps|tctss|t.timestamps|
|validates||validates :column, presence: true|
|add_column||add_column :table, :column, :type|
|add_reference||add_reference :table, :column, foreign_key: true|
|**Feature**|||

## Params
|Prefix||
|---|---|
|params|params.require(:id_name).permit(:variable)|
|require|require(:id_name)|
|permit|permit(:id_name)|

## Controller
|Prefix|shortcut||
|---|---|---|
|controller||class Controller < ApplicationController<br> <br>end|
|index||def index<br><br>end|
|create||def create<br><br>end|
|new||def new<br><br>end|
|edit||def edit<br><br>end|
|show||def show<br><br>end|
|update||def update<br><br>end|
|destroy||def destroy<br><br>end|
|CRUD||def index<br><br>end<br><br>def new<br><br>end<br><br>def create<br><br>end<br><br>def edit<br><br>end<br><br>def update<br><br>end<br><br>def show<br><br>end<br><br>def destroy<br><br>end|
|before_action|ba|before_action :id|
## Others
|Prefix||
|---|---|
|if|if $1<br>&nbsp;&nbsp;$2<br>end|
|if else|if $1<br>&nbsp;&nbsp;$2<br>else<br>&nbsp;&nbsp;$3<br>end|
|if elsif|if $1<br>&nbsp;&nbsp;$2<br>elsif $3<br>&nbsp;&nbsp;$4<br>end|
|if elsif else|if $1<br>&nbsp;&nbsp;$2<br>elsif $3<br>&nbsp;&nbsp;$4<br>else<br>&nbsp;&nbsp;$5<br>end|
|first|first(quantity)|
|find_by|find_by(id: params[:id])|
|where|where(condition)|
|increment|increment(:id)|
|order|order(id: :desc)|
|limit|limit(quantity)|
|def|def {name}<br><br>end|


***If have any advice,use [GitHub Issue](https://github.com/VenseChang/vscode-rails/issues) or <a href="mailto:vense1023@gmail.com?subject=[VSCode Extension%20-%20Rails%20Snippets]%20">mail</a> to  me.***

# Link
- [GitHub](https://github.com/Drunces/vscode-rails)
- [Marketplace](https://marketplace.visualstudio.com/items?itemName=Vense.rails-snippets)

---
### Enjoy it!


