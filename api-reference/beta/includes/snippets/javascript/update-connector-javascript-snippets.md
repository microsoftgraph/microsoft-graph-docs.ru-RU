---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a9c6c93c363ef94ae38b8ea2087293f53827c78
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printConnector = {
  displayName: 'ConnectorName',
  fullyQualifiedDomainName: 'CONNECTOR-MACHINE',
  operatingSystem: 'Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555',
  appVersion: '0.19.7338.23496',
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

await client.api('/print/connectors/{id}')
    .version('beta')
    .update(printConnector);

```