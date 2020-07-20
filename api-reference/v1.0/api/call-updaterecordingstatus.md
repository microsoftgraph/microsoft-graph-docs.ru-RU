---
title: 'Call: Упдатерекордингстатус'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: bb8f68f53453662d8ab0707138c011548379a4e6
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183969"
---
# <a name="call-updaterecordingstatus"></a>Call: Упдатерекордингстатус

Пространство имен: microsoft.graph

Обновление состояния записи приложения, связанного с вызовом. Для этого необходимо использовать решение для [записи на основе политики Teams](https://docs.microsoft.com/MicrosoftTeams/teams-recording-policy) .

> **Дополнительное ограничение**: вы не можете использовать API-интерфейс для записи или сохранения мультимедийного контента из вызовов или собраний, к которым обращается приложение, или данных, полученных из этого контента ("запись" или "запись"), без предварительного вызова API **упдатерекордингстатус** для указания того, что запись началась и получает ответ об успешной отправке от этого API. Если приложение начинает запись собрания, оно должно закончить запись перед вызовом API **упдатерекордингстатус** , чтобы указать, что запись закончена.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)      |
|:---------------------------------------|:-------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                                    |
| Приложение                            | Calls. Жоинграупкаллс. ALL, Calls. Акцессмедиа. ALL  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр       | Тип    | Описание                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| Контекст   | Строка  | Уникальная строка контекста клиента. Максимальный лимит — 256 символов.                                 |
| status          | String  | Состояние записи. Возможные значения: `notRecording` , `recording` , или `failed` .  |

## <a name="response"></a>Отклик
Этот метод возвращает `200 OK` код отклика и заголовок Location с URI для объекта [упдатерекордингстатусоператион](../resources/updaterecordingstatusoperation.md) , созданного для этого запроса.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a>Отклик

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateRecordingStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
