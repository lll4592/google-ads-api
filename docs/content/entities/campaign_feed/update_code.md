---
title: Update CampaignFeed
order: 5.1
type: update_code
entity: CampaignFeed
---

```javascript
// Updating the entity

const campaign_feed = {
  resource_name: 'customers/9262111890/campaignFeeds/1483704368~82896692', // The resource_name is required
  // ...any other fields that you would like to update
}

// Passing in a single entity to update
const result = await customer.campaignFeeds.update(campaign_feed)

// Passing in an array of entities to update, validating only
const result = await customer.campaignFeeds.update([campaign_feed, other_campaign_feed], {
  validate_only: true,
})
```

```javascript

// Example result
{
	results : ['customers/9262111890/campaignFeeds/1483704368~82896692'],
	partial_failure_error : null,
	request: { /* your request object */ }
}

```
