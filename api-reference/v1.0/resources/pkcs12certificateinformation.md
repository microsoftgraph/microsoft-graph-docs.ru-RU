---
title: тип ресурса pkcs12CertificateInformation
description: Представляет общедоступные сведения клиентского сертификата Pkcs12.
author: nickgmicrosoft
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5b5374d65d462c3ea016b2fa19684f939851e748
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007001"
---
# <a name="pkcs12certificateinformation-resource-type"></a>тип ресурса pkcs12CertificateInformation

Пространство имен: microsoft.graph

Представляет общедоступные сведения сертификата Pkcs12.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isActive|Логический|  Представляет, является ли сертификат активным сертификатом, используемым для вызова соединиттеля API. Активный сертификат — это самый недавно загруженный сертификат, срок действия которого еще не истек, но срок которого не истек.|
|отпечатки пальцев|Строка| Отпечаток сертификата. |
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
