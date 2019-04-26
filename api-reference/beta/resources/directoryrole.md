---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Дополнительные сведения о ролях каталогов (администратора) см. в разделе Назначение ролей администратора в Azure AD. С помощью Microsoft Graph вы можете назначить пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активирована только роль каталога администраторов компании. Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом directoryRoleTemplate, на котором основана роль каталога. Наследуется от directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 110febf3213431a0a44941a4cdd2bd9bca255bff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334602"
---
# <a name="directoryrole-resource-type"></a>Тип ресурса directoryRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Дополнительные сведения о ролях каталогов (администратора) см. [в разделе Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). С помощью Microsoft Graph вы можете назначить пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активирована только роль каталога администраторов компании. Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом [directoryRoleTemplate](directoryroletemplate.md) , на котором основана роль каталога. Наследуется от [directoryObject](directoryobject.md).

По умолчанию роли каталога разделяются на уровне клиента.  Однако роли каталогов (в настоящее время только *Администратор учетной записи пользователя* и *администратор службы поддержки*) также могут быть ограничены [административными единицами](administrativeunit.md).

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |Считывание свойств и отношений объекта directoryRole.|
|[Список перечисление directoryrole](../api/directoryrole-list.md) | Коллекция объектов [directoryRole](directoryrole.md) | Список ролей каталога, активированных в клиенте. |
|[Добавление участника](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Добавление пользователя в роль каталога путем записи данных в свойство навигации members.|
|[Перечисление участников](../api/directoryrole-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.|
|[Удаление участника](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Удаление пользователя из роли каталога.|
|[Область списка — элементы роли](../api/directoryrole-list-members.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| ПереЧислите членов этой роли каталога, область действия которой ограничена [административными единицами](administrativeunit.md), с помощью коллекции ресурсов scopedrolemembership изменен.|
|[delta](../api/directoryrole-delta.md)|Коллекция объектов directoryRole| Получение добавочных изменений для ролей каталога. |

## <a name="properties"></a>Свойства
| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание роли каталога. Только для чтения. |
|displayName|Строка|Отображаемое имя роли каталога. Только для чтения. |
|id|Строка|Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.|
|roleTemplateId|String| Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения. |

## <a name="relationships"></a>Отношения
| Отношение | Тип |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.|
|Scopedadministrators|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Члены этой роли каталога, областью действия которой являются [административные единицы](administrativeunit.md). Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
