---
title: 'synchronizationJob: Приостановка'
description: Временно приостановить синхронизации. Сохраняются все текущие, включая состояние задания и задание продолжит работу с где остановились при вызове Пуск.
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513923"
---
# <a name="synchronizationjob-pause"></a>synchronizationJob: Приостановка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Временно приостановить синхронизации. Сохраняются все текущие, включая состояние задания и задание продолжит работу с где оно было прервано Если [запустить](../api/synchronization-synchronizationjob-start.md) вызов.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     |Directory.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |Не поддерживается.  |
|Для приложений                            |Не поддерживается. | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Тип    | Описание|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

В случае успеха возвращает `204 No Content` ответа. Он не возвращает все действия в теле ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a>Ответ
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
