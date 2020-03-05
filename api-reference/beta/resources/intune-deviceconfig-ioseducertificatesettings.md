---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 503d2b1d0f4fa94e95d20882b10a0c30d968680e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529929"
---
# <a name="ioseducertificatesettings-resource-type"></a>Тип ресурса Иоседуцертификатесеттингс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|trustedRootCertificate|Binary|Доверенный корневой сертификат.|
|цертфиленаме|String|Имя файла, отображаемое в пользовательском интерфейсе.|
|цертификатионаусорити|String|Центр сертификации PKCS.|
|цертификатионаусоритинаме|String|Имя центра сертификации PKCS.|
|цертификатетемплатенаме|String|Имя шаблона сертификата PKCS.|
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



