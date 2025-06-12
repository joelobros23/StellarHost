# Project Plan: StellarHost

**Description:** A simplified web hosting platform enabling users to manage domains, plans, and basic server settings with a clean and intuitive interface.


## Development Goals

- [ ] Configure tailwindcss-rails and update application.tailwind.css for initial styling.
- [ ] Implement user authentication using Devise, enabling users to register, login, and manage their profiles.
- [ ] Modify the Domain model to include associations with the User model (belongs_to :user) and add validations for name, plan, and user_id.
- [ ] Update the Domains controller to ensure only logged-in users can create, edit, and view their own domains. Restrict access to domains belonging to other users.
- [ ] Customize the Domain scaffold views (index.html.erb, show.html.erb, new.html.erb, edit.html.erb) using Tailwind CSS for a modern and responsive design.
- [ ] Implement a simple 'Plan' model (or enum within the Domain model) with predefined hosting plan options (e.g., 'Basic', 'Standard', 'Premium').
- [ ] Display the user's domains on their profile page after they log in.
- [ ] Add basic error handling and user-friendly error messages for common actions (e.g., invalid domain name, plan selection).
- [ ] Set up the root route to a user dashboard page (if logged in) or a marketing landing page (if logged out).
- [ ] Implement a 'status' field for domains to represent their operational state (e.g., 'Active', 'Inactive', 'Suspended').
