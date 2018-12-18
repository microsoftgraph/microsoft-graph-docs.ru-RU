---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
ms.openlocfilehash: 1c77b3a33b19e9f0254642ef89e3d7fddc224b9a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320771"
---
# <a name="create-group"></a>Создание группы

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Используйте этот интерфейс API для создания новой [группы](../resources/group.md) , указанный в тексте запроса. Можно создать одну из трех типов групп:

* Группа Office 365 (единая группа)
* Динамическая группа
* Группа безопасности

> **Примечание**: чтобы создать [группы](../resources/team.md), сначала создайте группу затем добавьте группы, обратитесь к разделу [Создание группы](../api/team-put-teams.md).

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
В следующей таблице приведены свойства [группы](../resources/group.md) ресурса для указания при создании группы. 

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| displayName | строка | Имя, которое следует отобразить в адресной книге для группы. Обязательный. |
| mailEnabled | boolean | Устанавливает значение **true** для групп с включенной поддержкой почты. Установите значение **true,** Если создание группы с Office 365. Установите значение **false,** Если создание динамических или группу безопасности. Обязательный. |
| mailNickname | string | Почтовый псевдоним для группы. Обязательный. |
| securityEnabled | boolean | Значение **true** для группы с включенной поддержкой безопасности. Установите значение **true,** Если создание динамической или группу безопасности. При создании группы с Office 365, задайте это значение **false** . Обязательный. |
| owners | Коллекция строк | Это свойство представляет владельцев группы во время создания. Необязательный атрибут. |
| members | Коллекция строк | Это свойство представляет члены группы во время создания. Необязательный атрибут. |

При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.

| Тип группы | Свойство **groupTypes** |
|:--------------|:------------------------|
| Office 365 (как единая группа)| "Unified" |
| Динамическая группа | "DynamicMembership" |
| Система безопасности | Не следует устанавливать. |

Поскольку **группы** ресурсов поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в группе при его создании.

>**Примечание:** Создание группу Office 365 программными средствами без контекста пользователя и указание владельцев будет создать группу анонимных пользователей.  Это может привести к связанного сайта SharePoint Online, не создается автоматически до дальнейшей вручную действия предпринимаются.  

При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика.

## <a name="example"></a>Пример
#### <a name="request-1"></a>Запрос 1
Первый запрос пример создает группу Office 365.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a>Ответ
Ниже приведен пример ответа.
>**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>Запрос 2
Второй запрос на примере создает группу Office 365 с помощью указанных владельцев.
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json
 {
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a>Ответ 2
Ниже приведен пример успешного ответа.
>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
 {
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
