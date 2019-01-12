---
title: Тип ресурса groupSetting
description: Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, а также разрешение или запрещение пользователям-гостям быть владельцами групп.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911695"
---
# <a name="groupsetting-resource-type"></a>Тип ресурса groupSetting

Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, а также разрешение или запрещение пользователям-гостям быть владельцами групп.

Можно на базе доступных объектов [groupSettingTemplate](groupsettingtemplate.md) создавать параметры группы, а также менять предопределенные значения по умолчанию этих параметров. Они контролируют поведение групп на уровне клиента или отдельной группы. Если один и тот же параметр определен на двух уровнях — и клиента, и отдельной группы, параметр для группы переопределяет параметр для клиента.  Например, если получать приглашения от существующих членов групп разрешает пользователям параметр на уровне клиента, но запрещает параметр для отдельной группы, гости не смогут делать этого. Параметры группы контролируют только поведение групп Office 365.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. |
|[Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта параметра. |
|[Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов параметра. |
|[Обновление параметра](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Обновление объекта groupsetting. |
|[Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта параметра. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|String| Отображаемое имя этой группы параметров, которое получено с использованием связанного шаблона. |
|id|String| Уникальный идентификатор этих параметров. Только для чтения. |
|templateId|String| Уникальный идентификатор шаблона, который использовался для создания этой группы параметров. Только для чтения. |
|values|Коллекция объектов [settingValue](settingvalue.md)| Коллекция пар "имя-значение". Должно содержать и задавать все параметры, определенные в шаблоне. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
