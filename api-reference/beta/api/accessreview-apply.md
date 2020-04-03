---
title: Применение Акцессревиев
description: 'В функции проверок доступа Azure AD примените решения завершенной Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8b1866737ede1159fc955496eb1d2ceef6d650ad
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123568"
---
# <a name="apply-accessreview"></a>Применение Акцессревиев

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD примените решения завершенной [акцессревиев](../resources/accessreview.md).  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  


После завершения проверки доступа либо из-за того, что она достигла даты окончания, либо администратор остановил его вручную, и автоматическое применение не настроено для проверки, вы можете вызвать Apply, чтобы применить изменения. Пока не будет применено, решения для удаления прав доступа не будут отображаться в исходном ресурсе, пользователи для экземпляра сохраняют сведения о членстве в группах. Вызывая Apply, результат проверки реализуется путем обновления группы или приложения. Если в ходе рецензирования был запрещен доступ пользователя, то при вызове администратором этого API служба Azure AD удаляет членство или назначение приложения. 

После завершения проверки доступа и автоматического применения этого параметра Состояние проверки изменится с "завершено" на "промежуточные состояния", а "наконец" изменится на "применено состояние". Вы должны увидеть запрещенных пользователей (при их наличии), которые удаляются из назначения группы ресурсов или приложения в течение нескольких минут.

Настроенное автоматическое применение проверки или выбор применения не оказывает никакого действия для группы, созданной в локальном каталоге или в динамической группе. Если вы хотите изменить группу, которая является локальной, скачайте результаты и примените эти изменения к представлению группы в этом каталоге.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/applyDecisions
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.


## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.

## <a name="see-also"></a>См. также

- [Как выполнить проверку доступа](https://docs.microsoft.com/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
