---
title: Обновление ediscoveryReviewTag
description: Обновление свойств объекта ediscoveryReviewTag.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ceb490ed7c5fcd91d6e2b1625c70a3a417c076c8
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838390"
---
# <a name="update-ediscoveryreviewtag"></a>Обновление ediscoveryReviewTag
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags/{ediscoveryReviewTagId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя тега. Обязательный.|
|description|Строка|Описание тега. Необязательный элемент.|
|childSelectability|microsoft.graph.security.childSelectability|Это значение определяет, представляет ли пользовательский интерфейс теги как флажки или группу переключателей. Возможные значения: `One`, `Many`. Обязательный.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ediscoveryreviewtag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/062de822f17a4a2e9b833aa3f6c37108

{
    "displayName": "My tag API 2",
    "description": "Use Graph API to create tags (updated)"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoveryreviewtag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoveryreviewtag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ediscoveryreviewtag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-ediscoveryreviewtag-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content

```

