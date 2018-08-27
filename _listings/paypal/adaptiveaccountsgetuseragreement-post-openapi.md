---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 0
info:
  title: Paypal Get User Agreement
  description: The GetUserAgreement API operation lets you retrieve the user agreement
    for the customer to approve the new PayPal account.
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptiveAccounts/AddBankAccount:
    post:
      summary: Add Bank Account
      description: The AddBankAccount API operation lets your application set up bank
        accounts as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.AddBankAccount.post
      x-api-path-slug: adaptiveaccountsaddbankaccount-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Bank Account
  /AdaptiveAccounts/AddPaymentCard:
    post:
      summary: Add Payment Card
      description: The AddPaymentCard API operation lets your application set up credit
        cards as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.AddPaymentCard.post
      x-api-path-slug: adaptiveaccountsaddpaymentcard-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Credit Card
  /AdaptiveAccounts/CreateAccount:
    post:
      summary: Create Account
      description: The CreateAccount API operation enables you to create a PayPal
        account on behalf of a third party.
      operationId: AdaptiveAccounts.CreateAccount.post
      x-api-path-slug: adaptiveaccountscreateaccount-post
      parameters:
      - in: header
        name: X-PAYPAL-SANDBOX-EMAIL-ADDRESS
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptiveAccounts/GetUserAgreement:
    post:
      summary: Get User Agreement
      description: The GetUserAgreement API operation lets you retrieve the user agreement
        for the customer to approve the new PayPal account.
      operationId: AdaptiveAccounts.GetUserAgreement.post
      x-api-path-slug: adaptiveaccountsgetuseragreement-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Aggreements
  /AdaptiveAccounts/GetVerifiedStatus:
    post:
      summary: Get Verified Status
      description: The GetVerifiedStatus API operation lets you check if a PayPal
        account status is verified. A PayPal account gains verified status under a
        variety of circumstances, such as when an account is linked to a verified
        funding source. Verified status serves to indicate a trust relationship. For
        more information about account verified status, refer to PayPal.com.
      operationId: AdaptiveAccounts.GetVerifiedStatus.post
      x-api-path-slug: adaptiveaccountsgetverifiedstatus-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Verified
      - Status
  /AdaptiveAccounts/SetFundingSourceConfirmed:
    post:
      summary: Set Funding Source Confirmed
      description: The SetFundingSourceConfirmed API operation lets your application
        set up bank accounts as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.SetFundingSourceConfirmed.post
      x-api-path-slug: adaptiveaccountssetfundingsourceconfirmed-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Verified
      - Status
  /AdaptivePayments/CancelPreapproval:
    post:
      summary: Cancel Preapproval
      description: Use the CancelPreapproval API operation to handle the canceling
        of preapprovals. Preapprovals can be canceled regardless of the state they
        are in, such as active, expired, deactivated, and previously canceled.
      operationId: AdaptivePayments.CancelPreapproval.post
      x-api-path-slug: adaptivepaymentscancelpreapproval-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/ConvertCurrency:
    post:
      summary: Convert Currency
      description: Use the ConvertCurrency API operation to request the current foreign
        exchange (FX) rate for a specific amount and currency.
      operationId: AdaptivePayments.ConvertCurrency.post
      x-api-path-slug: adaptivepaymentsconvertcurrency-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Currency
  /AdaptivePayments/ExecutePayment:
    post:
      summary: Execute Payment
      description: The ExecutePayment API operation lets you execute a payment set
        up with the Pay API operation with the actionType CREATE. To pay receivers
        identified in the Pay call, set the pay key from the PayResponse message in
        the ExecutePaymentRequest message.
      operationId: AdaptivePayments.ExecutePayment.post
      x-api-path-slug: adaptivepaymentsexecutepayment-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/GetFundingPlans:
    post:
      summary: Get Funding Plans
      description: Use the GetFundingPlans API operation to determine the funding
        sources that are available for a specified payment, identified by its key,
        which takes into account the preferences and country of the receiver as well
        as the payment amount. You must be both the sender of the payment and the
        caller of this API operation
      operationId: AdaptivePayments.GetFundingPlans.post
      x-api-path-slug: adaptivepaymentsgetfundingplans-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Plans
  /AdaptivePayments/GetPaymentOptions:
    post:
      summary: Get Payment Options
      description: You use the GetPaymentOptions API operation to retrieve the payment
        options passed with the SetPaymentOptionsRequest.
      operationId: AdaptivePayments.GetPaymentOptions.post
      x-api-path-slug: adaptivepaymentsgetpaymentoptions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/GetShippingAddresses:
    post:
      summary: Get Shipping Addresses
      description: Use the GetShippingAddresses API operation to obtain the selected
        shipping address. You must have created the payment or preapproval key that
        identifies the account holder whose shipping address you want to obtain, or
        be the primary receiver of the payment or one of the parallel receivers of
        the payment. The shipping address is available only if it was provided during
        the embedded payment flow.
      operationId: AdaptivePayments.GetShippingAddresses.post
      x-api-path-slug: adaptivepaymentsgetshippingaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Addresses
  /AdaptivePayments/Pay:
    post:
      summary: Pay
      description: Use the Pay API operation to transfer funds from a sender???s PayPal
        account to one or more receivers??? PayPal accounts. You can use the Pay API
        operation to make simple payments, chained payments, or parallel payments;
        these payments can be explicitly approved, preapproved, or implicitly approved.
      operationId: AdaptivePayments.Pay.post
      x-api-path-slug: adaptivepaymentspay-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/PaymentDetails:
    post:
      summary: Payment Details
      description: Use the PaymentDetails API operation to obtain information about
        a payment. You can identify the payment by your tracking ID, the PayPal transaction
        ID in an IPN message, or the pay key associated with the payment.
      operationId: AdaptivePayments.PaymentDetails.post
      x-api-path-slug: adaptivepaymentspaymentdetails-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/Preapproval:
    post:
      summary: Preapproval
      description: 'Use the Preapproval API operation to set up an agreement between
        yourself and a sender for making payments on the sender???s behalf. You set
        up a preapprovals for a specific maximum amount over a specific period of
        time and, optionally, by any of the following constraints: the number of payments,
        a maximum per-payment amount, a specific day of the week or the month, and
        whether or not a PIN is required for each payment request.'
      operationId: AdaptivePayments.Preapproval.post
      x-api-path-slug: adaptivepaymentspreapproval-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/PreapprovalDetails:
    post:
      summary: Preapproval Details
      description: Use the PreapprovalDetails API operation to obtain information
        about an agreement between you and a sender for making payments on the sender???s
        behalf.
      operationId: AdaptivePayments.PreapprovalDetails.post
      x-api-path-slug: adaptivepaymentspreapprovaldetails-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/Refund:
    post:
      summary: Refund
      description: Use the Refund API operation to refund all or part of a payment.
        You can specify the amount of the refund and identify the accounts to receive
        the refund by the payment key or tracking ID, and optionally, by transaction
        ID or the receivers of the original payment.
      operationId: AdaptivePayments.Refund.post
      x-api-path-slug: adaptivepaymentsrefund-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Refunds
  /AdaptivePayments/SetPaymentOptions:
    post:
      summary: Set Payment Options
      description: "You use the SetPaymentOptions API operation to specify settings
        for a payment of the actionType CREATE. \n\t\t\t\t\tThis actionType is specified
        in the PayRequest message."
      operationId: AdaptivePayments.SetPaymentOptions.post
      x-api-path-slug: adaptivepaymentssetpaymentoptions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---