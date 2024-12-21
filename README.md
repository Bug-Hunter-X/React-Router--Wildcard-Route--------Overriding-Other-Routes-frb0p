# React Router Wildcard Route Issue

This repository demonstrates a common issue in React Router v6 where a wildcard route (`/*`) overrides more specific routes.  The problem arises when the wildcard route is defined after other routes, causing those routes to never be matched. This results in unexpected routing behavior, such as always redirecting to the wildcard component.

**Solution:** The correct order for the routes is crucial to avoid such conflicts.  Specific routes should always come *before* the wildcard route.
