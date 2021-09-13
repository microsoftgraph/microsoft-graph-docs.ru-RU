---
title: тип ресурса iosEduCertificateSettings
description: Доверенные сертификаты Root и PFX для iOS EDU.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d97070415d65f8193bcf69bbcf771cd59684ff4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047151"
---
# <a name="ioseducertificatesettings-resource-type"></a>тип ресурса iosEduCertificateSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Доверенные сертификаты Root и PFX для iOS EDU.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|trustedRootCertificate|В двоичном формате|Надежный корневой сертификат.|
|certFileName|String|Имя файла для отображения в пользовательском интерфейсе.|
|certificationAuthority|String|Сертификационный орган PKCS.|
|certificationAuthorityName|String|Имя органа сертификации PKCS.|
|certificateTemplateName|String|Имя шаблона шаблона сертификата PKCS.|
|renewalThresholdPercentage|Int32|Процент порогового значения обновления сертификата. Допустимые значения от 1 до 99|
|certificateValidityPeriodValue|Int32|Значение для срока действия сертификата.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Масштаб для срока действия сертификата. Возможные значения: `days`, `months`, `years`.|

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



