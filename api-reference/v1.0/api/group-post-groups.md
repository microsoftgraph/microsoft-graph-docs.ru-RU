---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: c82774e72e6841f84d879ce3ce34febb8d88c2fd
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353099"
---
# <a name="create-group"></a>Создание группы
Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:

* Группа Office 365 (единая группа)
* Динамическая группа
* Группа безопасности

Эта операция по умолчанию возвращает только часть свойств для каждой группы. Эти свойства указаны в разделе [Свойства](../resources/group.md#properties)

Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`. См. [пример](group-get.md#request-2).

> **Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы. 

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| displayName | string | Имя, которое следует отобразить в адресной книге для группы. Обязательный. |
| mailEnabled | boolean | Установите значение **true** для групп, поддерживающих почту. Установите значение **true** при создании группы Office 365. При создании динамической группы или группы безопасности установите для этого свойства значение **false**. Обязательный. |
| mailNickname | string | Почтовый псевдоним для группы. Обязательный. |
| securityEnabled | boolean | Установите значение **true** для защищенных групп. При создании динамической группы или группы безопасности установите для этого свойства значение **true**. Установите значение **false** при создании группы Office 365. Обязательный. |
| owners | Коллекция строк | Это свойство представляет владельцев группы на момент создания. Необязательный параметр. |
| members | Коллекция строк | Это свойство представляет участников группы на момент создания. Необязательный параметр. |


При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.

### <a name="grouptypes-options"></a>Параметры groupTypes

| Тип группы | Свойство **groupTypes** |
|:--------------|:------------------------|
| Office 365 (как единая группа)| "Unified" |
| Динамическая группа | "DynamicMembership" |
| Система безопасности | Не задавайте. |


>**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.  Это может привести к тому, что связанный с ней сайт SharePoint Online, не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.  

При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика. Отклик включает в себя только свойства по умолчанию для группы.

## <a name="example"></a>Пример
#### <a name="request-1"></a>Запрос 1
Первый пример запроса создает группу Office 365.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a>Ответ 1
Ниже приведен пример ответа.
>**Примечание.** Показанный здесь объект ответа может быть сокращен для удобства чтения. В результате реального вызова возвращаются все свойства по умолчанию.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
      "deletedDateTime": null,
      "classification": null,
      "createdDateTime": "2018-12-22T00:51:37Z",
      "creationOptions": [],
      "description": "Self help community for library",
      "displayName": "Library Assist",
      "groupTypes": [
          "Unified"
      ],
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a>Запрос 2
Второй пример запроса создает группу Office 365 с указанным владельцем.
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a>Ответ 2
Ниже представлен пример успешного ответа. Он включает только свойства по умолчанию. Вы можете получить свойство навигации группы **owners**, чтобы проверить информацию о владельце. 
>**Примечание.** Показанный здесь объект ответа может быть сокращен для удобства чтения. В результате реального вызова возвращаются все свойства по умолчанию.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
