---
title: Тип ресурса securityVendorInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512180"
---
# <a name="securityvendorinformation-resource-type"></a>Тип ресурса securityVendorInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|Поставщик |String|Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.|
|providerVersion|String|Версия поставщика или subprovider, если он существует, создавшее оповещение. *Required*|
|subProvider|String|Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.|
|поставщика |String|Имя оповещения поставщика (например, Microsoft, Dell, FireEye). *Required*|

## <a name="json-representation"></a>Представление JSON

Соответствовать является представлением JSON ресурса.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
