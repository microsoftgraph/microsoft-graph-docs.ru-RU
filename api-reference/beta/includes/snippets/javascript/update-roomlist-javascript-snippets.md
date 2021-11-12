---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c3fe10c0e678b35ee05c1f6c141f6120201940c52612a17f42292fef8f7b865
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57204916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  '@odata.type': 'microsoft.graph.roomList',
  displayName: 'Building 1',
  phone: '555-555-0100',
  address: {
    street: '4567 Main Street',
    city: 'Buffalo',
    state: 'NY',
    postalCode: '98052',
    countryOrRegion: 'USA'
  },
  geoCoordinates: {
    altitude: null,
    latitude: 47.0,
    longitude: -122.0,
    accuracy: null,
    altitudeAccuracy: null
 }
};

await client.api('/places/Building1RroomList@contoso.onmicrosoft.com')
    .version('beta')
    .update(place);

```