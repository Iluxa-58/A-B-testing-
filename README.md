# A/B Test: Advertising Impact on User Conversion

## Project goal

The goal of this project is to evaluate whether an advertising campaign increased user conversion compared to a control group.

The project simulates a real product analytics task: not only checking statistical significance, but also making a business recommendation based on the size and reliability of the effect.

## Dataset

I used the Marketing A/B Testing dataset from Kaggle.

The dataset contains users split into two groups:

- `ad`: users who saw the advertisement
- `psa`: users who saw a public service announcement instead of the ad

The target variable is `converted`, which shows whether the user converted.

## Business question

Should the company continue running the ad campaign?

## Metrics

Primary metric:

- Conversion rate

Additional checks:

- Group balance
- Conversion by day
- Conversion by hour
- Confidence interval
- Practical significance

## Methodology

1. Load and clean the data
2. Compare sample sizes between groups
3. Calculate conversion rate for each group
4. Estimate absolute and relative uplift
5. Run a two-proportion z-test
6. Build a bootstrap confidence interval
7. Check conversion patterns by day and hour
8. Make a business recommendation

## Final decision

The final recommendation is based on both statistical significance and practical significance.
