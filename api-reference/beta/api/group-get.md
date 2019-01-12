---
title: Вывод группы
description: Получение свойств и связей объекта группы.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 99215af564be186edaf57563ae493f363c9cc2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941053"
---
# <a name="get-group"></a>Вывод группы

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получите свойства и связи объекта [группы](../resources/group.md) .

##### <a name="default-properties"></a>Свойства по умолчанию

Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении групп или выводе списка групп. Это подмножество всех доступных свойств. 

* classification
* createdDateTime
* description
* displayName
* groupTypes
* id
* mail
* mailEnabled
* mailNickname
* membershipRule
* membershipRuleProcessingState
* onPremisesLastSyncDateTime
* onPremisesSecurityIdentifier
* onPremisesSyncEnabled
* preferredLanguage - не поддерживается; значение для этого свойства не может быть набора и возвращает `null` при вызове.
* proxyAddresses
* renewedDateTime
* securityEnabled
* темы
* visibility

По умолчанию следующие свойства групп не возвращаются:

* accessType
* allowExternalSenders
* autoSubscribeNewMembers
* hasMembersWithLicenseErrors
* isSubscribedByMail
* isFavorite
* unseenConversationsCount
* unseenCount
* unseenMessagesCount

Для получения этих свойств (за исключением **isFavorite** и **hasMembersWithLicenseErrors**), воспользуйтесь `$select` параметр запроса. Ниже представлены примеры. 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

Чтобы вернуть группы, содержащие элементы с ошибками лицензии, используйте параметр **$filter** запроса:

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

Поскольку **группы** ресурсов поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **группы** .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. 
>**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения. При фактическом вызове будут возвращены все свойства по умолчанию, как описано ранее.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
