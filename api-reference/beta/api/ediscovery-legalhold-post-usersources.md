---
title: Создание legalHold userSource
description: Создание нового объекта legalHold userSource.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0c89d9428b48e3e35d5da0a4e43218ed44de14a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986725"
---
# <a name="create-legalhold-usersource"></a>Создание legalHold userSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавляет userSource в объект legalHold.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем JSON-представление [объекта userSource.](../resources/ediscovery-usersource.md)

В следующей таблице показаны свойства, необходимые при создании [userSource.](../resources/ediscovery-usersource.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|SMTP-адрес пользователя или SMTP-адрес группового почтового ящика. Чтобы получить адрес электронной почты группы, используйте [группы List или](../api/group-list.md) Get [group.](../api/group-get.md) Используя группу get, можно запрашивать по имени группы `$filter` с помощью; например, `https://graph.microsoft.com/v1.0/groups?$filter=displayName eq 'secret group'&$select=mail,id,displayName` . |
|includedSources|microsoft.graph.ediscovery.sourceType|Указывает, какие источники включены в эту группу. Это значение должно быть `mailbox` , `site` не поддерживается для legalHolds в настоящее время.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources
Content-Type: application/json

{
  "email": "adelev@contoso.com",
  "includedSources": "mailbox"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-usersource-from--2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalholds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-12-28T20:08:57.857Z",
            "id": "2192ca40-8ea2-410e-ba3b-ec8ae873be6b",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "EDiscovery admin"
                }
            }
        }
    ]
}
```
