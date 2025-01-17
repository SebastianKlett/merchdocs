---
title: Products in Category
---

The Products in Category section lists the products that are currently assigned to the category{% if "Default.CE Only" contains site.edition %}.{% endif %}{% if "Default.EE-B2B" contains site.edition %}, and allows you to use [category rules]({{ site.baseurl }}{% link catalog/category-product-rules.md %}) to dynamically change the product selection when a set of conditions is met.{% endif %}{% if "Default.CE Only" contains site.edition %}The search filters at the top of each column are used to add and remove products from the category.{% endif %}{% if "Default.EE-B2B" contains site.edition %}To learn more, see: [Visual Merchandiser]({{ site.baseurl }}{% link marketing/visual-merchandiser.md %}).{% endif %}

<!--{% if "Default.CE Only" contains site.edition %}-->
![]({{ site.baseurl }}{% link images/images/category-products-in-category.png %}){: .zoom}
<!--{% endif %}-->
<!--{% if "Default.EE-B2B" contains site.edition %}-->
![]({{ site.baseurl }}{% link images/images-ee/category-products-in-category.png %}){: .zoom}
<!--{% endif %}-->
*Category Products*

<!--{% if "Default.EE-B2B" contains site.edition %}-->
## To apply a category rule:

1. Set **Match products by rule** to the “Yes” position.

   The automatic sorting and condition options appear.

   ![]({{ site.baseurl }}{% link images/images-ee/category-match-products-by-rule.png %}){: .zoom}
   *To Match Products by Rule*

   **Automatic Sort**

   To apply a sort order automatically to the list, based on current conditions, set **Automatic Sorting** to one of the following:

   | Stock level | Move to top or bottom. |
   | Special price | Move to top or bottom. |
   | New Products | List newest products first. |
   | Color | Sort alphabetically by color. |
   | Name | Sort in ascending or descending order by Name. |
   | SKU | Sort in ascending or descending order by SKU |
   | Price | Sort in ascending or descending order by Price. |
   {:style="table-layout:auto"}

   **Add Condition**

   1. Tap <span class="btn">Add Condition</span>, Then, do the following:

      * Choose the **Attribute** that is the basis of the condition.
      * Choose the **Operator** that is needed to form the expression.
      * Enter the **Value** that is to be matched.

      ![]({{ site.baseurl }}{% link images/images-ee/category-rule-create.png %}){: .zoom}
      *Add Condition to Category Rule*

   1. Repeat this process for each attribute that is needed to describe the condition(s) to be met. For example, to match products that were created between 7 and 30 days ago, do the following:

      * Set **Date Created** to “Less than 30”.
      * Set **Logic** to “AND”.
      * Set **Date Modified** to “Greater than 7”.

1. When complete, tap <span class="btn">Save Category</span>.

{:.bs-callout .bs-callout-tip}
When setting up a category rule, the products are matched and assigned to the rule when the category is saved. Therefore, if you add a new product to the catalog and want to include it in the rule, you must re-save each category that is set to match products by rule, to ensure that the new product is included.

<table>
<col WIDTH="200">
<col WIDTH="auto">
         <thead>
            <tr>
               <th>Option</th>
               <th>Description</th>
            </tr>
         </thead>
         <tbody>
            <tr>
               <td>Match products by rule</td>
               <td>Determines if the list of products in the category is dynamically generated by a category rule. Options: Yes / No</td>
            </tr>
            <tr>
               <td>Automatic Sorting</td>
               <td>Automatically applies a sorting order to the list of category products. Options: None, Move low stock to top, Move low stock to bottom, Special price to top, Special price to bottom, Newest products first, Sort by color, Name: A - Z, Name: Z - A, SKU: Ascending, SKU: Descending, Price: High to Low, Price: Low to High</td>
            </tr>
            <tr>
               <td>Add Condition</td>
               <td>Adds an additional condition to the rule.</td>
            </tr>
            <tr>
               <td colspan="2"><i>Conditions</i></td>
            </tr>
            <tr>
               <td>Attribute</td>
               <td>Determines the attribute that is used as the basis of the condition. Options:<table>
               <col WIDTH="200">
               <col WIDTH="auto"><tbody><tr><td>Clone Category ID(s)</td><td>Dynamically clones products from multiple categories based on Category ID.</td></tr><tr><td>Color</td><td>Includes products based on color.</td></tr><tr><td>Date Created (days ago)</td><td>Includes products based on the number of days since the products were added to the catalog.</td></tr><tr><td>Date Modified (days ago)</td><td>Includes products based on the number of days since the products were last modified.</td></tr><tr><td>Name</td><td>Includes products based on the product name.</td></tr><tr><td>Price</td><td>Includes products based on price.</td></tr><tr><td>Quantity</td><td>Includes products based on the quantity in stock.</td></tr><tr><td>SKU</td><td>Includes products based on SKU.</td></tr></tbody></table></td>
            </tr>
            <tr>
               <td>Operator</td>
               <td>Specifies the operator that is applied to the attribute value to meet the  condition. Unless an operator is specified, “Equal” is used as the default. Options: Equal, Not equal, Greater than, Greater than or equal to, Less than, Less than or equal to, Contains</td>
            </tr>
            <tr>
               <td>Value</td>
               <td>Specifies the value  the attribute must have to meet the condition.</td>
            </tr>
            <tr>
               <td>Logic</td>
               <td>The Logic column is used to define multiple conditions, and appears only when an additional condition is added. Options: OR / AND</td>
            </tr>
         </tbody>
      </table>
<!--{% endif %}-->

<table>
      <h3 class="TableHeading">Workspace Controls</h3>
      <col WIDTH="200">
      <col WIDTH="auto">
      <thead>
         <tr>
            <th>Control</th>
            <th>Description</th>
         </tr>
      </thead>
      <tbody markdown="1">
         <!--{% if "Default.EE-B2B" contains site.edition %}-->
         <tr>
            <td>
               <p>
                  <img src="{{ site.baseurl }}{% link images/images/btn-view-as-list.png %}" class="button_height" />
               </p>
            </td>
            <td>View as List</td>
         </tr>
         <tr>
            <td>
               <img src="{{ site.baseurl }}{% link images/images/btn-view-as-tiles.png %}" class="button_height" />
            </td>
            <td>View as Tiles</td>
         </tr>
         <tr>
            <td>
               <img src="{{ site.baseurl }}{% link images/images/btn-no.png %}" class="button_height" />
               <img src="{{ site.baseurl }}{% link images/images/btn-yes.png %}" class="button_height" />
            </td>
            <td>Match by Rule</td>
         </tr>
         <tr>
            <td>
               <p>
                  <img src="{{ site.baseurl }}{% link images/images/btn-drag.png %}" />
               </p>
            </td>
            <td>The drag and drop control allows you to grab a product and move it to another position in the current page of the grid. To learn more, see: <a href="{{ site.baseurl }}{% link marketing/visual-merchandiser.md %}">Visual Merchandiser</a>.</td>
         </tr>
         <tr>
            <td>
               <img src="{{ site.baseurl }}{% link images/images/btn-position.png %}" class="button_height" />
            </td>
            <td> Determines the position of the product in the list. </td>
         </tr>
         <!--{% endif %}-->
         <!--{% if "Default.CE Only" contains site.edition %}-->
         <tr>
            <td markdown="1">
               <p class="tableBody">
                  <img src="{{ site.baseurl }}{% link images/images/btn-checkbox.png %}" class="button_height" />
               </p>
            </td>
            <td>The checkbox in the header of the first column can be used to select or deselect all products. The control in the first row determines the type of search, and can be set to include any record, or only those that are either assigned or not assigned to the category. The checkbox in the first column of each row identifies products to be added to the category. Options: Yes / No / Any</td>
         </tr>
         <tr>
            <td>Search Filters</td>
            <td>The <a href="{{ site.baseurl }}{% link stores/admin-grid-controls.md %}">filter controls</a> at the top of each column can be used to enter specific values you want to either include or omit from the list, depending on the Select All setting.</td>
         </tr>
         <tr>
            <td>Reset Filter</td>
            <td>Clears all search filters.</td>
         </tr>
         <tr>
            <td>Search</td>
            <td>Searches the catalog based on the filter criteria, and displays the result.</td>
         </tr>
         <!--{% endif %}-->
      </tbody>
   </table>
