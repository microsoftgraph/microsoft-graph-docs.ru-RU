---
title: Тип ресурса Директорисеттинг
description: Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес и заменены заданными по умолчанию стилями. Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов. Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.  Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы. Параметры, заданные в системе, управляют поведением групп Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535252"
---
# <a name="directorysetting-resource-type"></a>Тип ресурса Директорисеттинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры каталога могут быть созданы на основе доступных [директорисеттингтемплатес](directorysettingtemplate.md)и заменены заданными по умолчанию стилями. Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов. Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.  Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы. Параметры, заданные в системе, управляют поведением групп Office.

> **Note**: версия/Beta типа ресурса директорисеттинг применяется только к группам. Версия/v1.0 переименована в groupSetting.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание параметра](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Создание объекта Setting на основе объекта Директорисеттингтемплате. Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.|
|[Получение параметра](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Считывание свойств определенного объекта setting.|
|[Перечисление параметров](../api/directorysetting-list.md) | Коллекция [directorySetting](directorysetting.md) |Перечисление свойств всех объектов setting.|
|[Обновление параметра](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Обновление объекта setting. В обновлении можно изменить только Сеттингвалуес.|
|[Удаление параметра](../api/directorysetting-delete.md) | Нет |Удаление объекта setting. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|string|Отображаемое имя группы параметров, поступающих из связанного шаблона. Только для чтения.|
|id|строка| Уникальный идентификатор для этих параметров. Только для чтения.|
|templateId|string| Уникальный идентификатор шаблона, который используется для создания этой группы параметров. Только для чтения.|
|values|Коллекция [settingValue](settingvalue.md)| Коллекция пар "имя-значение". Должен содержать и задавать все параметры, определенные в шаблоне.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
