---
title: Тип ресурса publishedResource
description: Тип ресурса publishedResource.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1090e985fc9ffdec0c27f9793a361851d2fa5216
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155568"
---
# <a name="publishedresource-resource-type"></a>Тип ресурса publishedResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локально опубликованный ресурс. Администратор клиента может публиковать различные типы локального ресурса — корпоративные приложения, контроллеры домена, серверы и [т.](onpremisesagent.md) д. Установленные администратором клиента локально агенты можно настроить для доступа к определенному опубликованного ресурса и обработки запросов.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список publishedResources](../api/publishedresource-list.md) | [Коллекция объектов publishedResource](publishedresource.md) | Получите **коллекцию объектов publishedResources.** |
| [Get publishedResource](../api/publishedresource-get.md) | [publishedResource](publishedresource.md) | Чтение свойств и связей объекта **publishedResource.** |
| [Создание publishedResource](../api/publishedresource-post.md) |  [publishedResource](publishedresource.md)  | Создание нового **publishedResource**. |
| [Обновление publishedResource](../api/publishedresource-update.md) | [publishedResource](publishedresource.md) | Обновление объекта **publishedResource.** |
| [Удаление publishedResource](../api/publishedresource-delete.md) | Нет | Удаление объекта **publishedResource.** |
| [Назначение publishedResource onPremisesAgentGroup](../api/publishedresource-post-agentgroups.md) | Нет | **Назначьте объект publishedResource** **объекту onPremisesAgentGroup.** |
| [Удаление publishedResource из onPremisesAgentGroup](../api/publishedresource-delete-agentgroups.md) | Нет |  Удаление объекта **publishedResource** из **onPremisesAgentGroup.**|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String| Отображаемого имени publishedResource.|
|id|String| ИД объекта publishedResource. Только для чтения.|
|publishingType|string| Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|
|resourceName|String|Имя publishedResource.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|agentGroups|[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)| Список **onPremisesAgentGroups,** которые **назначены publishedResource.** Только для чтения. Допускается значение null.|

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


