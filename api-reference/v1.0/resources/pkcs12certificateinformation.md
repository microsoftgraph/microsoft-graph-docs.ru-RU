---
title: тип ресурса pkcs12CertificateInformation
description: Представляет общедоступные сведения клиентского сертификата Pkcs12.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6b0fe760be0fb67a92d99bbb53125cb79ad9204daf7484f5b8f2292f70a7fea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235368"
---
# <a name="pkcs12certificateinformation-resource-type"></a>тип ресурса pkcs12CertificateInformation

Пространство имен: microsoft.graph

Представляет общедоступные сведения сертификата Pkcs12.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isActive|Логическое|  Представляет, является ли сертификат активным сертификатом, используемым для вызова соединиттеля API. Активный сертификат — это самый недавно загруженный сертификат, срок действия которого еще не истек, но срок которого не истек.|
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
    "isActive": "Boolean",
    "thumbprint": "String",
    "notAfter": "DateTime",
    "notBefore": "DateTime"
}
```
