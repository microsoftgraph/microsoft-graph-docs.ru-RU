---
title: тип ресурса groupSetting
description: Параметры группы контролируют поведение, например заблокированные списки слов для имен отображения групп или разрешено ли гостевых пользователей быть владельцами групп.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 56d97a0789c33c429dcce7d5db7009f439806768
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084547"
---
# <a name="groupsetting-resource-type"></a>тип ресурса groupSetting

Пространство имен: microsoft.graph

Параметры группы контролируют поведение, например заблокированные списки слов для имен отображения групп или разрешено ли гостевых пользователей быть владельцами групп.

Параметры группы можно создать на основе доступных [группSettingTemplates](groupsettingtemplate.md)и изменить их по умолчанию. Эти параметры регулируют групповое поведение на уровне клиента или определенной группе. Если один и тот же параметр определяется как для клиента, так и для определенной группы, параметр группового уровня переопределяет параметр на уровне клиента.  Например, параметр для клиента может разрешить приглашать гостей существующими членами групп, но отдельные параметры группы могут переопределять и не разрешая приглашать гостей членами группы. Параметры группы регулируют только поведение Microsoft 365 групп.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Создание объекта настройки на основе groupSettingTemplate. Запрос POST должен предоставить параметрValues для всех параметров, определенных в шаблоне. |
|[Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта setting. |
|[Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов setting. |
|[Обновление параметра](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Обновление объекта groupsetting. |
|[Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта параметра. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|Строка| Отображение имени этой группы параметров, которое происходит из связанного шаблона. |
|id|String| Уникальный идентификатор для этих параметров. Только для чтения. |
|templateId|String| Уникальный идентификатор для шаблона, используемого для создания этой группы параметров. Только для чтения. |
|values|[settingValue](settingvalue.md) collection| Коллекция пар значений имен. Необходимо содержать и задать все параметры, определенные в шаблоне. |

## <a name="relationships"></a>Связи

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

