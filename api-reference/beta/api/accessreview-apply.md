---
title: Применение Акцессревиев
description: 'В функции проверок доступа Azure AD примените решения завершенной Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456880"
---
# <a name="apply-accessreview"></a>Применение Акцессревиев

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD примените решения завершенной [акцессревиев](../resources/accessreview.md).  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  


После завершения проверки доступа либо из-за того, что она достигла даты окончания, либо администратор остановил его вручную, и автоматическое применение не настроено для проверки, вы можете вызвать Apply, чтобы применить изменения. Пока не будет применено, решения для удаления прав доступа не будут отображаться в исходном ресурсе, пользователи для экземпляра сохраняют сведения о членстве в группах. Вызывая Apply, результат проверки реализуется путем обновления группы или приложения. Если в ходе рецензирования был запрещен доступ пользователя, то при вызове администратором этого API служба Azure AD удаляет членство или назначение приложения. 

После завершения проверки доступа и автоматического применения этого параметра Состояние проверки изменится с "завершено" на "промежуточные состояния", а "наконец" изменится на "применено состояние". Вы должны увидеть запрещенных пользователей (при их наличии), которые удаляются из назначения группы ресурсов или приложения в течение нескольких минут.

Настроенное автоматическое применение проверки или выбор применения не оказывает никакого действия для группы, созданной в локальном каталоге или в динамической группе. Если вы хотите изменить группу, которая является локальной, скачайте результаты и примените эти изменения к представлению группы в этом каталоге.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
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

- [Как выполнить проверку доступа](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
