---
title: тип ресурса teamsTabConfiguration (Open Type)
description: Параметры, определяя содержимое вкладки.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 90d9d51cffec818a601e8b7efddb4b77b1c2dc3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052862"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>тип ресурса teamsTabConfiguration (Open Type)

Пространство имен: microsoft.graph



Параметры, определяя содержимое [вкладки.](teamstab.md) При интерактивной настройке вкладки эта информация устанавливается приложением-поставщиком вкладок.
В дополнение к свойствам, перечисленным ниже, некоторые приложения-поставщики вкладок указывают дополнительные настраиваемые свойства.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|-|-|-|
|  entityId   |   string |  Идентификатор для объекта, принимающего поставщика вкладок.     |
|  contentUrl |   string |  URL-адрес, используемый для отрисовки содержимого вкладок в Teams. Обязательный.    |
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

