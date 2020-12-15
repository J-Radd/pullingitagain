# pullingitagain
// Set your secret key. Remember to switch to your live secret key in production!
// See your keys here: https://dashboard.stripe.com/account/apikeys
StripeConfiguration.ApiKey = "sk_live_...4kUR";

var options = new PayoutCreateOptions
{
  Amount = 10000,
  Currency = "usd",
  Method = "instant",
};

var requestOptions = new RequestOptions();
requestOptions.StripeAccount = "{{po_1HofeDJtofXoPBKRYs4jGaA0}}";

var service = new PayoutService();
var payout = service.Create(options, requestOptions);
