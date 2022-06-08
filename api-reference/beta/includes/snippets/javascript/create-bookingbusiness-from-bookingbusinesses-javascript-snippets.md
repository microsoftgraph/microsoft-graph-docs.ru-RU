---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53204cba6f51803aea1a8b2728c63e1cdbcc7c77
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65947048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingBusiness = {
    displayName: 'Fourth Coffee',
    address: {
        postOfficeBox: 'P.O. Box 123',
        street: '4567 Main Street',
        city: 'Buffalo',
        state: 'NY',
        countryOrRegion: 'USA',
        postalCode: '98052'
    },
    phone: '206-555-0100',
    email: 'manager@fourthcoffee.com',
    webSiteUrl: 'https://www.fourthcoffee.com',
    defaultCurrencyIso: 'USD'
};

await client.api('/bookingBusinesses')
    .version('beta')
    .post(bookingBusiness);

```