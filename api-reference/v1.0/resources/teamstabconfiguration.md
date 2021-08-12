---
title: тип ресурса teamsTabConfiguration (Open Type)
description: Параметры, определяя содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7a1af503a2ba4788f22d3c7d7a76b968d1d66c167c3138ef316d056abf2f800b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196489"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>тип ресурса teamsTabConfiguration (Open Type)

Пространство имен: microsoft.graph



Параметры, определяя содержимое [вкладки.](teamstab.md) При интерактивной настройке вкладки эта информация устанавливается приложением-поставщиком вкладок.
В дополнение к свойствам, перечисленным ниже, некоторые приложения-поставщики вкладок указывают дополнительные настраиваемые свойства.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|-|-|-|
|  entityId   |   string |  Идентификатор для объекта, принимающего поставщика вкладок.     |
|  contentUrl |   string |  URL-адрес, используемый для отрисовки содержимого вкладок в Teams. Обязательный элемент.    |
|  removeUrl  |   строка |  Url-адрес Teams клиентом при удалении вкладки с помощью Teams клиента.     |
|  websiteUrl |   string |  URL-адрес для показа содержимого вкладок за пределами Teams.     |

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

