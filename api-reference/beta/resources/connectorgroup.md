---
title: Тип ресурса Коннекторграуп
description: Представляет прокси приложения Коннекторграуп.
localization_priority: Normal
ms.prod: microsoft-identity-platform
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 446dae5e78878ba9648d532d2696b0bfde496601
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556172"
---
# <a name="connectorgroup-resource-type"></a>Тип ресурса Коннекторграуп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Каждый соединитель [прокси приложения Azure AD](https://aka.ms/whyappproxy) всегда является частью группы соединителей. Все соединители, принадлежащие одной и той же группе соединителей, действуют как отдельные единицы для обеспечения высокого уровня доступности и балансировки нагрузки. Если вы не создадите группы соединителей, все соединители будут входить в группу по умолчанию. При настройке приложения с помощью прокси для приложения также необходимо указать группу соединителей, которой необходимо назначить приложение.

После создания группы соединителей можно добавить или переместить соединители в группу соединителей с помощью [Add Connector](../api/connectorgroup-post-members.md). Вы также можете использовать [Add Application](../api/connectorgroup-post-applications.md) , чтобы назначить приложение для группы соединителей.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список Коннекторграуп](../api/connectorgroup-list.md) |Коллекция [коннекторграуп](connectorgroup.md) | Получение списка объектов Коннекторграуп. |
|[Получение Коннекторграуп](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | Чтение свойств и связей объекта Коннекторграуп. |
|[Обновление Коннекторграуп](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| Обновление объекта Коннекторграуп. |
|[Удаление Коннекторграуп](../api/connectorgroup-delete.md) | Нет | Удаление объекта Коннекторграуп. Прежде чем Коннекторграуп можно будет удалить, необходимо удалить все соединители из Коннекторграуп. |
|[Перечисление участников](../api/connectorgroup-list-members.md) |Коллекция [соединителей](connector.md)| Получение коллекции объектов Connector. |
|[Перечисление приложений](../api/connectorgroup-list-applications.md) |Коллекция [application](application.md)| Получение коллекции объектов Application, связанной с Коннекторграуп. |
|[Добавление приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Свяжите приложение с Коннекторграуп, размещая в коллекции Applications. |
|[Добавить соединитель](../api/connectorgroup-post-members.md) |[PDIF](connector.md)| Добавление соединителя в Коннекторграуп путем публикации в коллекции Коннекторграуп. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|коннекторграуптипе|string| Указывает тип гибридного агента. Это предварительно заданное системой. Только для чтения. |
|id|строка| Уникальный идентификатор для этого Коннекторграуп. Только для чтения. |
|isDefault|boolean| Указывает, является ли Коннекторграуп Коннекторграуп по умолчанию. Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предопределена системой. Только для чтения. |
|name|string| Имя, связанное с Коннекторграуп. |
|региональных|string| Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для. Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один из соединителей или приложений** . Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии. Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|заявлен|Коллекция [application](application.md)| Только для чтения. Допускается значение null.|
|members|Коллекция [соединителей](connector.md)| Только для чтения. Допускается значение null.|

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
