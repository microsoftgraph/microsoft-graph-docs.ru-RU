---
title: Тип ресурса Публишедресаурце
description: Тип ресурса Публишедресаурце.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841362"
---
# <a name="publishedresource-resource-type"></a>Тип ресурса Публишедресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локальный опубликованный ресурс. Администратор клиента может публиковать различные типы локальных ресурсов, корпоративных приложений, контроллеров домена, серверов и т. д. [локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к ним и обработки запросов к определенный опубликованный ресурс.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Публишедресаурцес](../api/publishedresource-list.md) | Коллекция объектов [публишедресаурце](publishedresource.md) | Получение коллекции объектов **публишедресаурцес** . |
| [Получение Публишедресаурце](../api/publishedresource-get.md) | [Публишедресаурце](publishedresource.md) | Чтение свойств и связей объекта **публишедресаурце** . |
| [Создание Публишедресаурце](../api/publishedresource-post.md) |  [Публишедресаурце](publishedresource.md)  | Создание нового **публишедресаурце**. |
| [Обновление Публишедресаурце](../api/publishedresource-update.md) | [Публишедресаурце](publishedresource.md) | Обновление объекта **публишедресаурце** . |
| [Удаление Публишедресаурце](../api/publishedresource-delete.md) | Нет | Удаление объекта **публишедресаурце** . |
| [Назначение Публишедресаурце для Онпремисесажентграуп](../api/publishedresource-post-agentgroups.md) | Нет | Назначьте объект **публишедресаурце** для **онпремисесажентграуп**. |
| [Удаление Публишедресаурце из Онпремисесажентграуп](../api/publishedresource-delete-agentgroups.md) | Нет |  Удаление объекта **публишедресаурце** из объекта **онпремисесажентграуп**.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка| Отображаемое имя Публишедресаурце.|
|id|String| Идентификатор объекта Публишедресаурце. Только для чтения.|
|Публишингтипе|string| Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.|
|resourceName|String|Имя Публишедресаурце.|

## <a name="relationships"></a>Отношения

| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|Ажентграупс|Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)| Список **онпремисесажентграупс** , которым назначено **публишедресаурце** . Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
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
