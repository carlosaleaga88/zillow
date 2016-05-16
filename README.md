Zillow, PHP Wrapper
================================

This is a simple PHP Wrapper for the Zillow API services.

Installation
------------

Add ``dfreer/zillow`` as a require dependency in your ``composer.json`` file:

.. code-block:: bash

    php composer.phar require dfreer/zillow:~1.0

Usage
-----

    use Zillow\ZillowClient;

    $client = new ZillowClient('ZWSID');

Make requests with a specific API call method:

    // Run GetSearchResults
    $response = $client->GetSearchResults(['address' => '5400 Tujunga Ave', 'citystatezip' => 'North Hollywood, CA 91601']);

Any Zillow API call will work. Valid callbacks are:

- GetZestimate
- GetSearchResults
- GetChart
- GetComps
- GetDeepComps
- GetDeepSearchResults
- GetUpdatedPropertyDetails
- GetDemographics
- GetRegionChildren
- GetRegionChart
- GetRateSummary
- GetMonthlyPayments
- CalculateMonthlyPaymentsAdvanced
- CalculateAffordability
- CalculateRefinance
- CalculateAdjustableMortgage
- CalculateMortgageTerms
- CalculateDiscountPoints
- CalculateBiWeeklyPayment
- CalculateNoCostVsTraditional
- CalculateTaxSavings
- CalculateFixedVsAdjustableRate
- CalculateInterstOnlyVsTraditional
- CalculateHELOC


License
-------

MIT license.
