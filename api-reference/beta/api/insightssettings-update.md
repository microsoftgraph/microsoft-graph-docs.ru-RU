---
title: Сведения об обновлении
description: Обновление свойств объекта insightsSettings
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: dcf841ce7b5da1b5796d8a86fb6e6be5e0e58bf5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096424"
---
# <a name="update-insightssettings"></a>Обновление insightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновим параметры конфиденциальности, чтобы отобразить или вернуть указанный тип данных в организации. Тип параметров может быть элементом проницательности или понимание людей.

Дополнительные сведения о настройке конфиденциальности для вашей организации см. в этой информации:
-  [Настройка конфиденциальности элементов](/graph/insights-customize-item-insights-privacy) 
-  [Настройка конфиденциальности для пользователей](/graph/insights-customize-people-insights-privacy)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из следующих разрешений. Дополнительные дополнительные информации, в том числе о выборе разрешений, см. [в см. в .](/graph/permissions-reference)

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |


>**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли глобального администратора.
## <a name="http-request"></a>HTTP-запрос

Обновление параметров для анализа элементов:
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

Чтобы обновить параметры для понимания людей:
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/peopleInsights
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Логический| `true` если для организации включен указанный тип анализа; если указанный тип анализа отключен для `false` всех пользователей без исключений. Значение по умолчанию: `true`. Необязательно.|
|disabledForGroup|Строка| ID группы Azure AD, в которой указанный тип данных отключен для ее участников. Значение по умолчанию: `empty`. Необязательный параметр.|

>**Примечание:** Эта операция не проверяет значение **свойства disabledForGroup,** если оно включено в тело запроса. Если задайте **свойство disabledForGroup** строке, эта операция не проверяет наличие соответствующей группы Azure AD. Это означает, что если вы установите **disabledForGroup** в группу Azure AD, которая не существует или удаляется после этого, эта операция не сможет идентифицировать членство в группе и отключить сведения о элементе или пользователях для определенных пользователей. Если **установлено isEnabledInOrganization,** операция позволит получить указанный тип данных для всех пользователей `true` организации.  
## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект insightsSettings](../resources/insightssettings.md) в тексте ответа.

## <a name="examples"></a>Примеры 

### <a name="example-1-update-settings-for-item-insights"></a>Пример 1. Обновление параметров для анализа элементов
#### <a name="request"></a>Запрос

Вот пример запроса, который показывает, как администратор обновляет параметр конфиденциальности **"disabledForGroup",** чтобы запретить отображать сведения о элементах пользователей в определенной группе Azure AD.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_insightssettings_iteminsightrequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-insightssettings-iteminsightrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-insightssettings-iteminsightrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-insightssettings-iteminsightrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-insightssettings-iteminsightrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-insightssettings-iteminsightrequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-insightssettings-iteminsightrequest-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "update_insightssettings_iteminsightrequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


### <a name="example-2-update-settings-for-people-insights"></a>Пример 2. Обновление параметров для понимания людей
#### <a name="request"></a>Запрос

Ниже приводится пример запроса, который показывает, как администратор обновляет параметр конфиденциальности **"disabledForGroup",** чтобы запретить отображать сведения о пользователях в определенной группе Azure AD.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_insightssettings_peopleinsightsrequest"
}-->
```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/peopleInsights
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-insightssettings-peopleinsightsrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-insightssettings-peopleinsightsrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-insightssettings-peopleinsightsrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-insightssettings-peopleinsightsrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-insightssettings-peopleinsightsrequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-insightssettings-peopleinsightsrequest-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.insightsSettings",
  "name": "update_insightssettings_peopleinsightsrequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


 107 api-reference/beta/api/iteminsightsettings-get.md 
