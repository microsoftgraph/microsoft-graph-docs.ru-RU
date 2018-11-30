---
title: Тип ресурса directoryRole
description: Представляет роль directory Azure AD. Каталог роли Azure AD также называются *ролями администратора*. Дополнительные сведения о ролях каталогов (администратор) в разделе назначение ролей администратора в Azure AD. Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступных каталогов, отправьте запрос POST с Идентификатором directoryRoleTemplate, лежащие в основе роли каталога. Наследуется от directoryObject.
ms.openlocfilehash: c3def9f75b62db1f07c648fed18f57f92f5c7f77
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076848"
---
# <a name="directoryrole-resource-type"></a>Тип ресурса directoryRole

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет роль directory Azure AD. Каталог роли Azure AD также называются *ролями администратора*. Дополнительные сведения о ролях каталогов (администратор) можно [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступных каталогов, отправьте запрос POST с Идентификатором [directoryRoleTemplate](directoryroletemplate.md) , лежащие в основе роли каталога. Наследуется от [directoryObject](directoryobject.md).

По умолчанию каталог роли распространяются всей клиента.  Тем не менее каталог роли (в настоящее время только *администратора учетной записи пользователя* и *администратора служба технической поддержки*) может также областью действия [администратора единиц измерения](administrativeunit.md).

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |Считывание свойств и отношений объекта directoryRole.|
|[Перечисление объектов directoryRole](../api/directoryrole-list.md) | Коллекция объектов [directoryRole](directoryrole.md) | Перечисление ролей каталога, активированных в клиенте. |
|[Добавление элемента](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Добавление пользователя в роль каталога путем записи данных в свойство навигации members.|
|[Список членов](../api/directoryrole-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.|
|[Удаление члена](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Удаление ресурса user из роли каталога.|
|[Список элементов области определения роли](../api/directoryrole-list-members.md) |[scopedRoleMembership](scopedrolemembership.md) коллекции| Список пользователей, которым эта роль каталогов, предназначенные для [администрирования единиц измерения](administrativeunit.md), через коллекцию ресурсов scopedRoleMembership.|
|[delta](../api/directoryrole-delta.md)|Коллекция объектов directoryRole| Получите добавочные изменения для каталога ролей. |

## <a name="properties"></a>Свойства
| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|описание|String|Описание роли каталога. Только для чтения. |
|displayName|String|Отображаемое имя роли каталога. Только для чтения. |
|id|String|Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.|
|roleTemplateId|String| Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения. |

## <a name="relationships"></a>Связи
| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.|
|scopedMembers|[scopedRoleMembership](scopedrolemembership.md) коллекции| Члены этой роли каталога, предназначенные для [администрирования единиц измерения](administrativeunit.md). Только для чтения. Допускается значение null.|

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
