---
title: Удаление участника
description: Удаление определенного участника в вызове.
manager: zhengni
author: jackry6350
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dfa5bc7454b2cd6c495502ee455d3872e54dfce4
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667782"
---
# <a name="delete-participant"></a>Удаление участника

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пространство имен: microsoft.graph

Удаление определенного участника в вызове. В некоторых ситуациях приложение может удалить участника из активного вызова. Это действие можно сделать до или после ответа участника на вызов. При удалении активного вызываемого звонка он немедленно удаляется из вызова без предварительного или после удаления уведомления. При удалении приглашенного участника отменяется любой незаявимый запрос на добавление участника.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                               |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | Нет                                        |

Конфигурация собрания на уровне клиента требуется для того, чтобы позволить приложению вызывать этот API. Администратор клиента должен вызвать следующий комдлет на удаленной PowerShell клиента, чтобы предоставить приложению разрешение на вызов этого API. Дополнительные сведения см. [в рублях Set-CsApplicationMeetingConfiguration.](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md)
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/participants/{id}
DELETE /communications/calls/{id}/participants/{id}
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-cancel-active-participant"></a>Пример 1. Отмена активного участника

#### <a name="request"></a>Запрос
Ниже показан пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-cancel-invited-non-active-participant"></a>Пример 2. Отмена приглашенного неавтного участника

#### <a name="invite-a-participant-to-an-existing-call"></a>Приглашение участника на существующий вызов

<!-- {
  "blockType": "request",
  "name": "participant-invite-1"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/invite
Content-Type: application/json
Content-Length: 464

{
  "participants": [
    {
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD"
        }
      }
    }
  ],
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f"
}
```

#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "eec3812a-fdc3-4fb4-825c-a06c9f35414e",
  "status": "Running",
  "clientContext": "f2fa86af-3c51-4bc2-8fc0-475452d9764f",
  "resultInfo": null,
  "participants": [
    {
      "endpointType": null,
      "id": null,
      "replacesCallId": "a7ebfb2d-871e-419c-87af-27290b22e8db",
      "identity": {
        "user": {
          "id": "278405a3-f568-4b3e-b684-009193463064",
          "identityProvider": "AAD",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47"
        },
        "application": null,
        "device": null,
        "phone": null
      }
    }
  ]
}
```

#### <a name="delete-invited-participant-before-participant-is-added-to-the-roster"></a>Удаление приглашенного участника до того, как участник будет добавлен в реестр

<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```

#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
