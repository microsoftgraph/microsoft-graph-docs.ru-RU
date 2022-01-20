---
title: тип ресурсов connectorGroup
description: Представляет соединители прокси-приложения.
ms.localizationpriority: medium
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: b5fc35d95479d8671ba4fd15f47f6beb857b9448
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088923"
---
# <a name="connectorgroup-resource-type"></a>тип ресурсов connectorGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Каждый [соединитатель прокси-сервера приложения Azure AD](/azure/active-directory/app-proxy/what-is-application-proxy) всегда является частью группы соединители. Все соединители, принадлежащие к одной группе соединитетелей, выступают в качестве отдельного блока для балансировки высокой доступности и нагрузки. Если вы не создаете соединители группы, все соединители будут частью группы по умолчанию. При настройке приложения с помощью прокси-сервера приложения необходимо также указать группу соединители для назначения приложения.

После создания группы соединителю можно добавить или переместить соединители в группу соединителю с помощью [соединитетеля Add.](../api/connectorgroup-post-members.md) Вы также можете использовать [приложение Add для](../api/connectorgroup-post-applications.md) назначения приложения группе соединителю.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Соединители спискиGroup](../api/connectorgroup-list.md) |[коллекция connectorGroup](connectorgroup.md) | Извлечение списка объектов connectorGroup. |
|[Создание connectorGroup](../api/connectorgroup-post.md) |[коллекция connectorGroup](connectorgroup.md) | Создание объекта connectorGroup. |
|[Получение connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | Чтение свойств и связей объекта connectorGroup. |
|[Обновление connectorGroup](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| Обновление объекта connectorGroup. |
|[Удаление connectorGroup](../api/connectorgroup-delete.md) | Нет | Удаление объекта connectorGroup. Все соединители должны быть удалены из соединителиГруппы, прежде чем соединителиGroup можно удалить. |
|[Список членов](../api/connectorgroup-list-members.md) |[коллекция соединители](connector.md)| Получите коллекцию объектов соединители. |
|[Перечисление приложений](../api/connectorgroup-list-applications.md) |Коллекция [application](application.md)| Получение коллекции объектов приложения, связанной с соединитетелемGroup. |
|[Добавление приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Связать приложение с соединителягруппой, разместив в коллекции приложений. |
|[Добавление соединителя](../api/connectorgroup-post-members.md) |[connector](connector.md)| Добавьте соединителю в соединителюGroup, разместив его в коллекции connectorGroup. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|connectorGroupType|connectorGroupType| Указывает тип гибридного агента. Это заранее заданной системой. Возможные значения: `applicationProxy` . Только для чтения. |
|id|string| Уникальный идентификатор для этого соединитетеляGroup. Только для чтения. |
|isDefault|boolean| Указывает, является ли соединительщикОм ConnectorGroup по умолчанию. Соединительщиком по умолчанию может быть только одна группа соединительных групп, и это заранее заданной системой. Только для чтения. |
|name|string| Имя, связанное с соединитетелемGroup. |
|регион|connectorGroupRegion| Регион, в который назначен connectorGroup, и будет оптимизировать трафик. Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительгруппе. Возможные значения: (для Северной `nam` **Америки),** `eur` (для Европы), `aus` (для Австралии), `asia` (для Азии), `ind` (для Индии) и `unknownFutureValue` .|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|приложения|Коллекция [application](application.md)| Только для чтения. Допускается значение null.|
|members|[коллекция соединители](connector.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->