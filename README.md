Follow LinkedIn Learning course [Learning App Building with Vanilla Javascript](https://www.linkedin.com/learning/learning-app-building-with-vanilla-javascript/) by [Sasah Vodnik](https://www.linkedin.com/learning/instructors/sasha-vodnik)

## Deploy to surge.sh

- Check available domain vanilajs.surge.sh  
  vanilajs.surge.sh

- Get deployment token

```bash
surge token
```

- Add deployment token to GitHub repository setting  
  SURGE_TOKEN=your-surge-deployment-token

```bash
# Set secret visible only to certain repositories
gh secret set SURGE_TOKEN --repos="vanillajs"
```

```bash
# Set domain you want to publish your site on https://your-surge-website-or-custom-domain.surge.sh
gh secret set SURGE_DOMAIN -b'vanilajs.surge.sh' --repos="vanillajs"
```
