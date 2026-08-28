# Book List Purchase Optimization Prompt

> **Note: You will need to update relevant shipping info such as [ZIP CODE], [STATE], [COUNTRY] for your use case. 

I have provided a Markdown file containing a list of books. Use the **provided Markdown file as the authoritative source for which books to purchase**.

## 1. Identify the books to purchase

* Only include books marked in the Markdown file with the **📑 bookmark-tabs / purchased marker** indicating that a physical copy was acquired.
* Do **not** include books that are only marked as having an online option.
* Do not add books that are not in the provided file.
* Preserve the title, edition, and ISBN from the file when identifying each book.
* If the file gives an edition range or says that multiple editions are acceptable, use the rules in the file when deciding which edition qualifies.

## 2. Search for current purchase options

For **every qualifying book**, search current listings from as many of these sellers/marketplaces as practical:

* Amazon
* **Amazon Prime**
* eBay
* Better World Books
* ThriftBooks
* AbeBooks
* Walmart
* Barnes & Noble
* Books-A-Million
* Half Price Books
* CampusBooks
* Alibris
* Other reputable book sellers/marketplaces if they offer a lower delivered price

Search by **ISBN first**, then verify the title, author, edition, and format. Do not assume that a listing with a similar title is the correct edition.

### Amazon requirement

Amazon and Amazon Prime must be checked explicitly.

Amazon prices frequently do not appear in normal web-search results. If Amazon's current price is not visible to the search system, **do not claim that Amazon was cheaper or more expensive**. Instead, report that the current Amazon price could not be independently verified.

If the user provides a current Amazon price, incorporate that price into the comparison and clearly identify it as **user-supplied** unless independently verified.

## 3. Acceptable condition

Only consider:

1. New
2. Used — Like New
3. Used — Very Good
4. Used — Good
5. Used — Ex-library
6. Used — Acceptable

Do **not** select Fair, Poor, damaged, incomplete, or otherwise inferior copies unless explicitly authorized.

When comparing used books, prefer the better condition when the delivered price difference is small.

## 4. Edition rule

If a **newer edition** of the requested book is available for **less than the delivered price of the listed edition**, use the newer edition.

However:

* Verify that it is actually a newer edition.
* Verify the ISBN.
* Verify that it is the same title/work and appropriate for the intended use.
* Clearly identify when an edition has been upgraded.
* Do not upgrade editions merely because the newer edition exists.
* If the newer edition costs more, keep the requested edition unless there is another reason to recommend the upgrade.

## 5. Shipping destination

Calculate shipping to:

**ZIP code: [ZIP CODE], [STATE], [COUNTRY]**

Shipping must be included in the comparison.

Use the actual shipping cost to ZIP code [ZIP CODE] whenever the seller provides it.

If shipping depends on order size, membership, or seller-specific thresholds, account for that when calculating the final basket cost.

Do **not** assume that shipping is free merely because a search result does not display a shipping charge.

## 6. IMPORTANT: Optimize by seller/basket, not by individual book

This is the most important requirement.

Do **not** simply select the cheapest individual listing for every book.

Instead, calculate the **total delivered cost of complete purchase baskets**.

For example:

* Seller A has Book 1 for $8 + $5 shipping.
* Seller B has Book 1 for $10 with free shipping.
* If the buyer is already purchasing $20+ of books from Seller A and therefore qualifies for free shipping, Book 1 may actually be cheaper through Seller A.

Therefore:

### First determine each seller's basket rules

For each seller, determine:

* Free-shipping threshold
* Standard shipping cost
* Per-item shipping, if applicable
* Combined shipping rules
* Prime/free-shipping rules
* Whether shipping varies by third-party seller
* Any membership requirements
* Whether the seller's shipping policy applies to the specific listing

Then determine the cheapest combination of sellers that purchases **all required books**.

### Basket optimization example

If:

| Seller      | Book price | Shipping |
| ----------- | ---------: | -------: |
| ThriftBooks |        $10 |    $2.39 |
| ThriftBooks |         $8 |    $2.39 |
| ThriftBooks |         $5 |    $2.39 |

and ThriftBooks offers free shipping at $20, the three books should be evaluated as a **$23 basket with $0 shipping**, not as three independent purchases.

Likewise, if moving a $10 book from one seller to another causes a shipping threshold to be lost, account for that change.

## 7. Compare complete basket combinations

For each plausible seller combination:

1. Assign each book to a seller.
2. Calculate the book subtotal for each seller.
3. Calculate that seller's actual shipping cost.
4. Apply free-shipping thresholds or membership benefits.
5. Calculate each seller's order total.
6. Add all seller order totals together.
7. Compare the complete basket against alternative combinations.

The objective is:

> **Minimize the total delivered cost of purchasing every required book.**

Do not optimize individual rows independently if doing so increases the total cost of the complete order.

## 8. Amazon Prime

Treat Amazon Prime shipping as **$0 shipping only when the specific listing is confirmed to be Prime eligible**.

Compare:

* Amazon New + Prime
* Amazon Used + Prime
* Amazon non-Prime
* Amazon third-party marketplace listings

A $21.93 new Prime copy, for example, should beat a $19.99 used copy with $6 shipping.

## 9. Seller and listing verification

For every selected listing, verify as much of the following as possible:

* Exact title
* Author
* Edition
* ISBN
* Format
* Condition
* Price
* Shipping
* Seller/vendor
* Prime/free-shipping eligibility
* Availability

Do not confuse different editions or formats such as:

* Hardcover vs paperback
* International edition vs U.S. edition
* Instructor edition
* Student edition
* Workbook vs textbook
* Loose-leaf edition
* Kindle/eBook vs physical book

## 10. Final output

Create a table with exactly these columns:

| Title | Condition (used good/used very good/new) | Best price found | Shipping | Total | Seller/Vendor | Notes | Price Checked (date/time) |
| ----- | ---------------------------------------- | ---------------: | -------: | ----: | ------------- | ----- | ------------------------- |

For **Condition**, use:

* New
* Used Like New
* Used Very Good
* Used Good
* Used Ex-library
* Used Acceptable

If the requested format requires only "used good/used very good/new," normalize the condition appropriately and explain any ambiguity in Notes.

### Notes should include useful information such as:

* ISBN
* Edition
* Newer edition used instead
* Amazon Prime status
* Seller-specific shipping threshold
* Whether shipping was verified for [ZIP CODE]
* User-supplied price vs independently verified price
* Any uncertainty about condition or shipping
* Why the selected listing beats another option

## 11. Add a seller-optimized purchase summary

After the main table, provide a second table:

| Seller | Books to purchase | Book Subtotal | Shipping | Order Total |
| ------ | ----------------- | ------------: | -------: | ----------: |

Group all books that should be purchased from the same seller into the same order whenever doing so reduces the total cost.

Then provide:

**Total books:** X
**Total book cost:** $X
**Total shipping:** $X
**Estimated sales tax:** $X or "not included"
**Total delivered cost before tax:** **$X**

## 12. Identify savings opportunities

After calculating the optimized basket, briefly explain:

* Which seller combinations produced the savings
* Which books were moved into a seller's basket specifically to reach free shipping
* Which Amazon Prime listings beat used marketplace listings
* Which newer editions were cheaper
* Which books were particularly difficult to source
* Any prices that need to be manually verified at checkout

## 13. Do not overstate certainty

Prices and inventory change frequently.

Clearly distinguish between:

* **Verified current price**
* **Search-result price**
* **User-provided current price**
* **Price that could not be independently verified**

If a marketplace does not expose destination-specific shipping, say so.

Do not invent shipping costs, Prime eligibility, seller names, conditions, or prices.

## 14. Final recommendation

The final answer should prioritize the **lowest realistic total cost for purchasing the complete book set**, not the lowest sticker price on individual books.

Before declaring the final total, perform one final check:

> **For every book, ask whether moving it into or out of another seller's basket would lower the total delivered cost of the entire order.**

This final basket-level check is mandatory.
