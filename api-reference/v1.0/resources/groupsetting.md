---
title: Тип ресурса groupSetting
description: Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570829"
---
# <a name="groupsetting-resource-type"></a>Тип ресурса groupSetting

Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.

Параметры группы могут быть созданы на основе доступных [граупсеттингтемплатес](groupsettingtemplate.md)и заменены заданными по умолчанию стилями. Эти параметры определяют поведение групп на уровне клиента или в определенной группе. Если один и тот же параметр определен как на уровне клиента, так и в определенной группе, то настройка уровня группы переопределяет параметр на уровне клиента.  Например, параметр на уровне клиента может разрешить гостям, которые будут приглашены существующими участниками группы, но параметр индивидуальной группы может переопределять и запрещать участникам группы приглашать гостей. Параметры группы управляют поведением только групп Office 365.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Создание объекта Setting на основе объекта groupSettingTemplate. Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне. |
|[Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта параметра. |
|[Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов параметра. |
|[Обновление параметра](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Обновление объекта groupsetting. |
|[Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта setting. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|String| Отображаемое имя группы параметров, поступающих из связанного шаблона. |
|id|String| Уникальный идентификатор для этих параметров. Только для чтения. |
|templateId|String| Уникальный идентификатор шаблона, который используется для создания этой группы параметров. Только для чтения. |
|values|Коллекция [settingValue](settingvalue.md)| Коллекция пар "имя-значение". Должен содержать и задавать все параметры, определенные в шаблоне. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
