---
title: Добавление accessReview редактор
description: 'В Azure AD access дается обзор компонента "," Обновление существующего объекта accessReview для добавления другого пользователя в качестве читателя.  Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов. Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516366"
---
# <a name="add-accessreview-reviewer"></a>Добавление accessReview редактор

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [accessReview](../resources/accessreview.md) для добавления другого пользователя в качестве читателя.  Эта операция допускается только рецензию доступа, который еще не завершено и только доступа рецензию где явным образом указаны рецензентов. Эта операция — это не разрешено рецензию доступа, в котором пользователи просмотрите собственные доступа и не предназначены рецензию доступа, назначенных группе владельцев как рецензентов. 


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
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Маркер носителя Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите JSON, представляющую идентификатор пользователя, который будет проверяющего.

В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении accessReview.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | Идентификатор пользователя.  |


## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201, Created` код ответа.

## <a name="example"></a>Пример

Это пример обновления одноразовый (не периодические) review доступа с дополнительной редактор.

##### <a name="request"></a>Запрос
В тексте запроса укажите JSON, представляющую идентификатор объекта пользователя.

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
