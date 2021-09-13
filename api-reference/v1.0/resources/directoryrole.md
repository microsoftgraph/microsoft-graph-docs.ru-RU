---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*.
ms.localizationpriority: high
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3effb90d2ddeffccd59de35b04295fc83b86e5f8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089748"
---
# <a name="directoryrole-resource-type"></a>Тип ресурса directoryRole

Пространство имен: microsoft.graph

Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles). С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для роли каталога. [Перечислите шаблоны для ролей каталогов](../api/directoryroletemplate-list.md), чтобы получить все остальные доступные роли каталогов. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) | Считывание свойств и отношений объекта directoryRole. |
|[Перечисление объектов directoryRole](../api/directoryrole-list.md) | Коллекция объектов [directoryRole](directoryrole.md) | Перечисление ролей каталога, активированных в клиенте. |
|[Добавление элемента](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Добавление пользователя в роль каталога путем записи данных в свойство навигации members.|
|[Список членов](../api/directoryrole-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.|
|[Удаление члена](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Удаление ресурса user из роли каталога.|
|[Активация directoryRole](../api/directoryrole-post-directoryroles.md) |[directoryRole](directoryrole.md) | Активация роли каталога.|
|[Перечисление объектов scopedMember](../api/directoryrole-list-scopedmembers.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| Перечисление участников этой роли каталога, относящихся к области [административных единиц](administrativeunit.md), с помощью коллекции ресурсов scopedRoleMembership.|
|[delta](../api/directoryrole-delta.md)|Коллекция объектов directoryRole| Получение добавочных изменений для ролей каталога. |

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|description|String|Описание роли каталога. Только для чтения. |
|displayName|Строка|Отображаемое имя роли каталога. Только для чтения. |
|id|Строка|Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.|
|roleTemplateId|String| Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения. |

## <a name="relationships"></a>Связи
| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.|
|scopedMembers|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Участники роли каталога, относящихся к области [административных единиц](administrativeunit.md). Только для чтения. Допускается значение NULL.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
