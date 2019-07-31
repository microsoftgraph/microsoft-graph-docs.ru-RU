---
title: 'educationSubmission: отзыв'
description: 'Указывает, что студенту требуется выполнить отправку. Это действие можно выполнить только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d37d34685aabe00bff82de453e68a8ebba36aa3a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955084"
---
# <a name="educationsubmission-recall"></a>educationSubmission: отзыв

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, что студенту требуется выполнить отправку. Это действие можно выполнить только студентом. Он изменит состояние отправки с "Отправлено" обратно на "работает".

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)             |
| :------------------------------------- | :------------------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | EduAssignments. Реадвритебасик, EduAssignments. ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                                           |
| Для приложений                            | Не поддерживается.                                          |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/recall
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

В приведенном ниже примере показано, как вызывать этот API.

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
