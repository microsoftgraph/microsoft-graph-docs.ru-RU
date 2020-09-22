---
title: Тип ресурса Теамстабконфигуратион (Open Type)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 449edfbbd04d0f691d89580829684cbe84b168d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046391"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>Тип ресурса Теамстабконфигуратион (Open Type)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, определяющие содержимое [вкладки](teamstab.md). При настройке вкладки в интерактивном режиме эти сведения задаются приложением поставщика вкладок.
Помимо приведенных ниже свойств, некоторые приложения поставщика вкладок задают дополнительные настраиваемые свойства.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|-|-|-|
|  entityId   |   string |  Идентификатор для сущности, размещенной у поставщика вкладок.     |
|  contentUrl |   string |  URL-адрес, используемый для отображения содержимого вкладки в Teams. Обязательный.    |
|  removeUrl  |   строка |  URL-адрес, вызываемый клиентом Teams при удалении вкладки с помощью клиента Teams.     |
|  websiteUrl |   string |  URL-адрес для отображения содержимого вкладки вне Teams.     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


