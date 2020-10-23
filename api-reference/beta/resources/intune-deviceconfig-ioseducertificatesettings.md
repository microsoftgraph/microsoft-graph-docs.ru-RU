---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2693075e10fc52536f130128dbadfb5d3f06c8ad
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726481"
---
# <a name="ioseducertificatesettings-resource-type"></a>Тип ресурса Иоседуцертификатесеттингс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|trustedRootCertificate|Binary|Доверенный корневой сертификат.|
|цертфиленаме|Строка|Имя файла, отображаемое в пользовательском интерфейсе.|
|цертификатионаусорити|Строка|Центр сертификации PKCS.|
|цертификатионаусоритинаме|Строка|Имя центра сертификации PKCS.|
|цертификатетемплатенаме|Строка|Имя шаблона сертификата PKCS.|
|Свойства renewalthresholdpercentage|Int32|Пороговое значение возобновления сертификата. Допустимые значения — от 1 до 99|
|certificateValidityPeriodValue|Int32|Значение срока действия сертификата.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Масштаб срока действия сертификата. Возможные значения: `days`, `months`, `years`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





