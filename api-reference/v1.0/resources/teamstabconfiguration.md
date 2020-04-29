---
title: Тип ресурса Теамстабконфигуратион (Open Type)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad6c3bcee979e10e308b307cec780c8ddc8950dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446837"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>Тип ресурса Теамстабконфигуратион (Open Type)

Пространство имен: microsoft.graph



Параметры, определяющие содержимое [вкладки](teamstab.md). При настройке вкладки в интерактивном режиме эти сведения задаются приложением поставщика вкладок.
Помимо приведенных ниже свойств, некоторые приложения поставщика вкладок задают дополнительные настраиваемые свойства.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|-|-|-|
|  entityId   |   string |  Идентификатор для сущности, размещенной у поставщика вкладок.     |
|  contentUrl |   string |  URL-адрес, используемый для отображения содержимого вкладки в Teams. Обязательный.    |
|  removeUrl  |   string |  URL-адрес, вызываемый клиентом Teams при удалении вкладки с помощью клиента Teams.     |
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
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
