---
title: Тип ресурса verifiedPublisher
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 5acc66bd72c65b25d8301c4870fa5ff0f98a0d73
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135627"
---
# <a name="verifiedpublisher-resource-type"></a>Тип ресурса verifiedPublisher

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет проверенного издателя [приложения.](application.md) Дополнительные сведения см. в [проверке Publisher.](/azure/active-directory/develop/publisher-verification-overview) Проверенные издатели устанавливаются с помощью [setVerifiedPublisher](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [unsetVerifiedPublisher.](../api/application-unsetverifiedpublisher.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|Строка|Проверенное имя издателя из учетной записи Microsoft Partner Network (MPN) издателя приложения.|
|verifiedPublisherId|Строка| ИД проверенного издателя из учетной записи Центра партнеров издателя приложений. |
|addedDateTime|DateTimeOffSet| Временнаямпетка первого или последнего обновления проверенного издателя. |


## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}

```


<!-- uuid: e9aa37e1-f0b7-4201-a6b2-d26ce091dff6
2020-09-09 20:42:32 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
