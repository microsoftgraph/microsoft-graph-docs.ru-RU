---
title: тип ресурса publishedResource
description: тип ресурса publishedResource.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: e55abdad4a03319407b1c6e31e37e717739f0d10
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941766"
---
# <a name="publishedresource-resource-type"></a>тип ресурса publishedResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локально опубликованный ресурс. Администратор клиента может публиковать различные типы локального ресурса — корпоративные приложения, контроллеры доменов, серверы и [т.](onpremisesagent.md) д. Агенты, установленные администратором клиента, могут быть настроены для доступа и обработки запросов к конкретному опубликованому ресурсу.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список опубликованныхResources](../api/publishedresource-list.md) | [коллекция объектов publishedResource](publishedresource.md) | Получите **коллекцию объектов publishedResources.** |
| [Get publishedResource](../api/publishedresource-get.md) | [publishedResource](publishedresource.md) | Ознакомьтесь с свойствами и отношениями объекта **publishedResource.** |
| [Создание publishedResource](../api/publishedresource-post.md) |  [publishedResource](publishedresource.md)  | Создание нового **publishedResource**. |
| [Update publishedResource](../api/publishedresource-update.md) | [publishedResource](publishedresource.md) | Обновление **объекта publishedResource.** |
| [Удаление publishedResource](../api/publishedresource-delete.md) | Нет | Удаление **объекта publishedResource.** |
| [Назначение publishedResource onPremisesAgentGroup](../api/publishedresource-post-agentgroups.md) | Нет | Назначение **объекта publishedResource** в **onPremisesAgentGroup.** |
| [Удаление publishedResource из onPremisesAgentGroup](../api/publishedresource-delete-agentgroups.md) | Нет |  Удалите **объект publishedResource** из **onPremisesAgentGroup.**|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка| Отображение имени опубликованногоРесурса.|
|id|Строка| ID объекта publishedResource. Только для чтения.|
|publishingType|Строка| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|
|resourceName|String|Имя опубликованногоResource.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|agentGroups|[коллекция onPremisesAgentGroup](onpremisesagentgroup.md)| Список **onPremisesAgentGroups,** которые **назначены публикацииResource.** Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


