Bug 1: route/auth.js
"await" was needed to retrieve information to authenticate user.

Bug 2: middleware/auth.js
jwt token would not verify with jwt.decode, I replaced it with jwt.verify

Bug 3: routes/users.js
GET request for findAll was returning all info about a user instead of basic information.

Bug 4: 
Added middleware requireAdmin to prohibit non-admin users to update another user