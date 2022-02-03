---
title: 'вызов: updateRecordingStatus'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ef8ea1bf9b5e48bba453addfe3e778856ce4126c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341197"
---
# <a name="call-updaterecordingstatus"></a>вызов: updateRecordingStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление состояния записи приложения, связанного с вызовом. Для этого необходимо использовать Teams [на основе политики записи](/MicrosoftTeams/teams-recording-policy).

> Дополнительное **ограничение. Вы** не можете использовать API доступа к мультимедиа для записи или иного сохраняемой медиаконтента из звонков или собраний, к которые ваше приложение получает доступ, или данных, полученных из этого медиаконтента ("запись" или "запись"), не вызывая сначала **API updateRecordingStatus**, чтобы указать, что запись началась, и получить ответ на успех от этого API. Если ваше приложение начинает записывать любое собрание, оно должно закончить запись перед вызовом **API updateRecordingStatus** , чтобы указать, что запись завершена.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)      |
|:---------------------------------------|:-------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается                                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                                    |
| Приложение                            | Calls.JoinGroupCalls.All, Calls.AccessMedia.All  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр       | Тип    | Описание                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| clientContext   | String  | Уникальная строка Client Context. Максимальное ограничение — 256 шаров.                                 |
| status          | String  | Состояние записи. Возможные значения: `notRecording`, `recording` или `failed`.  |

## <a name="response"></a>Отклик
Этот метод возвращает код `200 OK` ответа и загорелый загорелый код расположения с URI к объекту [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) , созданному для этого запроса.

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
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateRecordingStatus
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/call-updaterecordingstatus-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/call-updaterecordingstatus-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

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
