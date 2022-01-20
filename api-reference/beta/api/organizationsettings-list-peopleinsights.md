---
title: Список peopleInsights
description: Извлечение свойств объекта insightsSettings для отображения или возвращения понимания людей в организации.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 200d9f0daa1ce9a3d8b9facb2607b5f5ff4dc40d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125683"
---
# <a name="list-peopleinsights"></a>Список peopleInsights

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите свойства объекта [insightsSettings](../resources/insightssettings.md) для отображения или возвращения людей в организации.

Сведения о настройке конфиденциальности для людей в организации см. в примере [Customize people insights privacy](/graph/insights-customize-people-insights-privacy).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из следующих разрешений. Дополнительные дополнительные информации, в том числе о выборе разрешений, см. [в см. в .](/graph/permissions-reference)

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All, User.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/peopleInsights
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект insightsSettings](../resources/insightssettings.md) в тексте ответа.

## <a name="example"></a>Пример 
### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_insightssettingspeoplerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/peopleInsights
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-insightssettingspeoplerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-insightssettingspeoplerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-insightssettingspeoplerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-insightssettingspeoplerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-insightssettingspeoplerequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-insightssettingspeoplerequest-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика. 
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "get_insightssettingspeoplerequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```

## <a name="see-also"></a>См. также
[Настройка конфиденциальности элементов](/graph/insights-customize-item-insights-privacy) для организации.
