---
title: Тип ресурса Верифиедпублишер
description: Представляет проверенного издателя приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: 0285eb767a2fc4606dceaf74693a570f14dd6612
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471531"
---
# <a name="verifiedpublisher-resource-type"></a>Тип ресурса Верифиедпублишер

Пространство имен: microsoft.graph

Представляет проверенного издателя [приложения](application.md). Для получения дополнительных сведений см [Проверка издателя](https://docs.microsoft.com/azure/active-directory/develop/publisher-verification-overview). Проверенные издатели задаются с помощью [сетверифиедпублишер](../api/application-setverifiedpublisher.md) и могут быть удалены только с помощью [унсетверифиедпублишер](../api/application-unsetverifiedpublisher.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|String|Проверенное имя издателя из учетной записи центра партнера издателя приложения.|
|верифиедпублишерид|String| Идентификатор проверенного издателя из учетной записи центра партнера издателя приложения. |
|аддеддатетиме|DateTimeOffSet| Временная метка при первом добавлении проверенного издателя или последнего обновления. |


## <a name="json-representation"></a>Представление JSON
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


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
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
