### Creating an `ExecutorService` 

Expected time required: 15 min

We are developing new features for Amazon Prime Video. The feature we're working on today is to make a notification
alert when a video that the user has added to their watchlist is about to expire. A `Runnable` class,
`NotificationTask` has been created to send out the notifications based on different targets such as email,
mobile, and internet browser.  

Your job is to complete `NotificationManager` so the method `sendNotificationsOut` is able to complete its task by
submitting all three tasks to an `ExecutorService`.

Complete the implementation of the `NotificationManager` class by implementing the `sendSaleNotificationsOut()` method
so that it executes all `NotificationTask` instances in the provided `List`.

Verify that the test in `NotificationManagerTest` passes.