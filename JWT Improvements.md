-  **Token Expiration**:
    - [x]  Set an appropriate expiration time for JWT tokens to balance security and user convenience.
    - [x]  Ensure that expired tokens are properly handled and rejected.

-  **Token Refresh (Optional)**:
    - [ ]  Implement a token refresh mechanism to allow clients to obtain new access tokens without re-authenticating.
    - [ ]  Configure the token refresh flow in your OAuth server, including token expiration and refresh token storage.

-  **Token Revocation (Optional)**:
    - [ ]  Implement token revocation to invalidate tokens when necessary (e.g., user logout, security incident).
    - [ ]  Maintain a blacklist of revoked tokens on the server and check incoming tokens against this blacklist.

-  **Token Claims**:
    - [ ]  Review and optimize the claims (payload) included in your JWT tokens.
    - [ ]  Include only necessary claims to reduce token size and improve efficiency.
    - [ ]  Ensure that sensitive information is not included in the token payload.

-  **Token Validation**:
    - [ ]  Enhance token validation by checking issuer (`iss`) and audience (`aud`) claims to ensure tokens are used in the intended context.
    - [ ]  Implement stricter token validation rules based on your application's requirements.

-  **Security Considerations**:
    - [ ]  Safeguard your secret key (`SECRET_KEY`) used for signing JWT tokens.
    - [ ]  Use strong and unique secret keys for different environments (development, production).
    - [ ]  Consider rotating secret keys periodically for added security.

-  **Auditing and Logging**:
    - [ ]  Implement auditing and logging for token-related activities, such as token issuance, validation, and revocation.
    - [ ]  Monitor and log failed token validation attempts for security analysis.

-  **Token Scopes (Optional)**:
    - [ ]  Define and enforce token scopes to restrict the access and permissions associated with different tokens.
    - [ ]  Ensure that tokens are granted only the necessary permissions for specific operations.

-  **Cross-Origin Resource Sharing (CORS)**:
    - [ ]  Configure CORS settings to control which domains are allowed to make cross-origin requests to your server.
    - [ ]  Implement secure CORS policies to prevent unauthorized access.

-  **Token Storage on Client**:
    - [ ]  Determine the secure storage location for JWT tokens on the client (e.g., HTTP-only cookies, local storage, session storage).
    - [ ]  Be mindful of potential security risks, such as XSS attacks.

-  **Documentation and API Contracts**:
    - [ ]  Document the JWT-based authentication and authorization mechanism for your API users.
    - [ ]  Define clear API contracts for token issuance, validation, and usage.

-  **Testing and Validation**:
    - [ ]  Conduct thorough testing, including positive and negative scenarios, to validate your JWT functionality.
    - [ ]  Implement unit tests, integration tests, and security tests to ensure robustness.

-  **Security Best Practices**:
    - [ ]  Stay updated with security best practices related to JWTs and OAuth.
    - [ ]  Periodically review and update your JWT implementation to address any security vulnerabilities.

-  **User Experience**:
    - [ ]  Provide user-friendly error messages and guidance for handling expired or invalid tokens on the client side.

-  **Legal and Compliance**:
    - [ ]  Ensure that your JWT implementation complies with relevant data protection and privacy regulations, such as GDPR.

-  **Monitoring and Alerts**:
    - [ ]  Set up monitoring and alerts to detect and respond to unusual token activity or security incidents.

-  **Documentation and Training**:
    - [ ]  Train your development and operations teams on JWT and OAuth concepts, best practices, and troubleshooting.



income_statement : 
	breakdown 
	total_revenue 
	operating_revenue 
	cost_of_revenue 
	operating_expense 
	operating_income 
	net_income_common_stockholders 
	net_income 
	total_expenses 
	interest_income 
	interest_expense 
	net_interest_income 
	ebit 
	ebitda 


balance_sheet : 
	breakdown 
	total_assets 
	current_assets 
	cash_cash_equivalents_short_term_investments 
	cash_and_cash_equivalents 
	other_short_term_investments 
	receivables 
	accounts_receivable 
	other_receivables 
	total_liabilities_net_minority_interest 
	current_liabilities 
	payables_and_accrued_expenses 
	payables 
	accounts_payable 
	dividends_payable 
	other_payable 
	total_equity_gross_minority_interest 
	stockholders_equity 
	total_capitalization 

cash_flow :
	breakdown
	operating_cash_flow 
	investing_cash_flow 
	financing_cash_flow 
	free_cash_flow 


statistics :
	trailing_pe 
	price_sales 
	price_book 
	enterprise_value_ebitda 
	return_on_equity 
	quarterly_revenue_growth 
	quarterly_earnings_growth 
	total_debt_equity 
	forward_annual_dividend_yield 
	trailing_annual_dividend_yield 
	payout_ratio 
	interest_coverage_ratio 
	operating_cash_flow_net_income_ratio 
	free_cash_flow_conversion 
	debt_coverage_ratio 

price 