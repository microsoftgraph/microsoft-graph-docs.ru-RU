---
title: тип ресурса pkcs12CertificateInformation
description: Представляет общедоступные сведения клиентского сертификата Pkcs12.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ada0d5d56d9fc785f6056862324aebd69d7358b3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509401"
---
# <a name="pkcs12certificateinformation-resource-type"></a>тип ресурса pkcs12CertificateInformation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет общедоступные сведения сертификата Pkcs12.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isActive|Логический|  Представляет, является ли сертификат активным сертификатом, используемым для вызова соединиттеля API. Активный сертификат — это самый недавно загруженный сертификат, срок действия которого еще не истек, но срок которого не истек.|
|отпечатки пальцев|String| Отпечаток сертификата. |
|notAfter|Целое число| Срок действия сертификата. Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.)|
|notBefore|Целое число| Время выдачи сертификата (не ранее). Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.)|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": true,
    "thumbprint": "string",
    "notAfter": 0000000000,
    "notBefore": 0000000000,
}
```
