# java-paged-list
Automatically exported from code.google.com/p/java-paged-list

PagedList is a light-weight Java List implementation that works with a page size. Each time a fooList.get(i) is invoked, the list will check if it has fetched the page before containing that entry and will get the new page if necessary.

The PagedList works with an interface DataProvider, which is an interface that can be implemented by some database DAO for example. It could also be a service that gets it through SOAP, JMS or from a file. The PagedList doesn't care as long as it gets a DataProvider imlementation.
