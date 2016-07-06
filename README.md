# cerebral-orm

Cerebral is great, but it's not enough. It would be great to get more
features for building rich client side applications out of the box. In my mind,
these include:

* Offline application, that will sync when it gets online. Like
  Google Keep on your phone. The user of the application shouldn't
  have to worry about what is local and what is synced. It should only
  present itself to the user, if it can't sync for some reason.
* Typed and valid state, at all times. In the backend, we have SQL to
  help us make sure we can't save invalid data. Now, we have a mix of
  runtime validation (tcomb), compile time type checking (typescript),
  and data validation of state (action types). Instead, we should
  be able to say "All Users have these fields. If it does not, it is not valid"
* Easy to implement relationional data. Right now, we have to think *a lot* when
  about how to store our data (indexed by key), how to retrieve it, and how to 
  reference other data. We have different methods for retrieval and for updating.
  We have no standard specification for how to achieve this.

Overall, I want to make an idiot proof system. Or at least, not require so much
from the developer. Cerebral is a solid base, it's time to start building on top.

