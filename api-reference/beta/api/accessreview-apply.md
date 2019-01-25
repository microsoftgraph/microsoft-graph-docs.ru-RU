---
title: Применение accessReview
description: 'В Azure AD доступ к функции проверки, применение решения завершенных accessReview.  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512215"
---
# <a name="apply-accessreview"></a>Применение accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD применение решения завершенных [accessReview](../resources/accessreview.md).  Конечный объект может быть review однократного доступа или экземпляр повторяющейся проверки доступа.  


После завершения проверки доступа, либо так, как связаться с вами дату окончания или администратор остановлена вручную и автоматически назначаемой не был настроен на проверку, можно вызвать применить, чтобы применить изменения. Пока не происходит применить о решениях для удаления права доступа не отображаются на ресурсов источника, пользователей, например сохранять их членства в группе. Путем вызова применения, результат проверки реализована путем обновления группы или приложения. Если нет доступа пользователя в разделе review, когда администратор вызывает этот интерфейс API, Azure AD удалит их назначения членства или приложения. 

После проверки доступа по завершении работы и автоматически назначаемой был настроен, то состояние проверки будет заменен завершено промежуточного состояния и наконец изменится на состояние применения. При любой, удаляемого из ресурса групповой членства или приложение назначения всего за несколько минут должно привести для просмотра запрещенных пользователей.

Настроенные автоматическое применение проверки или выбор применить не влияет на группы, которая исходит в локальном каталоге или динамические группы. Если вы хотите изменить группу, которая исходит локальной, загрузите результаты и применить эти изменения к представление группы в этой папке.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
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
| Authorization | string | Маркер носителя Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.


## <a name="response"></a>Ответ
При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.

## <a name="see-also"></a>См. также

- [Инструкции для выполнения проверки доступа](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

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
