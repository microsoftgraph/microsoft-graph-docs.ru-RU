---
title: 'канал: provisionEmail'
description: Подготовка электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b2e619970c0cdadd574a4873cb3231a88934a087
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869626"
---
# <a name="channel-provisionemail"></a>канал: provisionEmail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставление адреса электронной почты для [канала](../resources/channel.md).

Microsoft Teams автоматически не содержит адрес электронной почты для канала по умолчанию. Чтобы Teams адрес электронной почты, можно вызвать **provisionEmail** или с помощью пользовательского интерфейса Teams, выберите get email address **,** который запускает Teams для создания адреса электронной почты, если он еще не был предварительно.

Чтобы удалить предварительный адрес электронной почты канала, используйте [метод removeEmail.](channel-removeemail.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированное (рабочая или учебная учетная запись)     | ChannelSettings.ReadWrite.All               |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Не поддерживается.                              |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/provisionEmail
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

Если электронная почта канала будет успешно продюсироваться, этот метод возвращает код ответа и объект `200 OK` [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) в тексте ответа. Предварительный адрес электронной почты находится в **свойстве электронной** почты.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_provisionemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-provisionemail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-provisionemail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-provisionemail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-provisionemail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
    "email": "1df8f174.teamsgraph.onmicrosoft.com@amer.teams.ms"
}
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Provision channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


