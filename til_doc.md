### 10/06/2020
In loading JavaScript file that needs to be loaded at the bottom of the HTML document, you can still include it in the head of a document if you add the attribute "defer"

When VSCode lint is complaining about an undefined variable that is just defined in a different file (like in Vue), you can define a fake global variable at the top of the file
``` /*global Vue */ ```

### 09/16/2020
Ruby builds the through table method to connect tables that have many-to-many relationships.
It is normally: 
```
def products
  category_products.map do |category_product|
    category_product.product
  end
end
```

But Rails writes this for you in your model rb file with:
```
has_many :categories, through: :category_products 
``` 

### 09/09/2020
Can condense code in controller file using scopes: https://www.rubyguides.com/2019/10/scopes-in-ruby-on-rails/. You essentially create your own function in the model file that you reference in the controller.

### 09/08/2020
Ruby ApplicationRecord class can set validationsfor user inputs. For example
```validates :first_name, presence: true```
will ensure the user entered a first_name parameter. You can provide error messages with
```@user.errors.full_messages```

### 09/07/2020
* Learned I can dry up views files using partial files. Referencing a partial file will reuse the JSON in there: ```render partial: "product.json.jb", locals: { product: @product }```
* Change Ruby on Rails databases with migration files and the Active Migration class. https://edgeguides.rubyonrails.org/active_record_migrations.html
* .new is a new domain that automatically opens new documents for the desired application. "sheet.new" opens a blank Google Sheets

### 09/03/2020
* Learned how to turn my API to a Restful API using naming conventions defined by

### 09/02/2020
Sensitive info parameters can be passed in an HTTP request using a POST method and instead of using the url to pass parameters, you use the HTTP body.

### 09/01/2020
The controller in Ruby on Rails inherits a variable called "params" that allows you to pull information from user URL parameters (the ? after the path). You would grab the query parameters like you would a hash, like `params["parameter_name"]`.

### 08/30/2020
Model, Viewer, Controller concepts in action using Ruby on Rails. I can run my own server from my computer AND can publish my own websites for free on GitHub

### 08/27/2020
- the great resource for random free APIs: https://mixedanalytics.com/blog/list-actually-free-open-no-auth-needed-apis/
- the tty-prompt Ruby gem that allows complex formatting for collecting user-inputs, like providing a list for the user to select from
- create a variable that is stored in your terminal environment and can be used in your code with ENV[VARIABLE]


### 08/26/2020
I learned about decomposition coding, break down into pieces and test.

### 08/25/2020
Today I learned I can use attr_reader, attr_writer, and attr_accessor to allow user to read, change, or both in your classes
`attr_reader :id, :fname, :lname`

### 08/24/2020
Terminal can run within VSCode

### 08/23/2020
Today I learned the JavaScript-style notation shortcut when assigning values to hash symbols.
`person1 = {fname: Megan, lname: White}`



