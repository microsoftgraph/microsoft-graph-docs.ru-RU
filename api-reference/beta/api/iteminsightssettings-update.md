---
title: Обновление itemInsights
description: Обновление свойств объекта itemInsightsSettings
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 0eb17d9e0a4f3285858800f32e6954bbd344dc27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053036"
---
# <a name="update-iteminsightssettings"></a>Обновление itemInsightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств указанного [ресурса itemInsightsSettings.](../resources/iteminsightssettings.md)

Сведения о настройке конфиденциальности элементов для организации см. в статье [Настройка конфиденциальности .](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0) 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

>**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли глобального администратора.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Логический| `true` если включена информация о элементах организации; `false` если сведения о элементах организации отключены для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательное.|
|disabledForGroup|String| ID группы Azure AD, из которой отключены сведения о элементах участников. Значение по умолчанию: `empty`. Необязательный параметр.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект itemInsightsSettings](../resources/iteminsightssettings.md) в тексте ответа.

>**Примечание:** Эта операция проверяет достоверность значений свойств указанного ресурса **itemInsightsSettings.** Если свойство **отключеноForGroup,** эта операция не проверяет наличие соответствующей группы Azure AD. Это означает, что если вы установите **disabledForGroup** в группу Azure AD, которая не существовала или была удалена после этого, эта операция не сможет идентифицировать членство в группе и отключить сведения о элементах для определенных пользователей. Если **установлено isEnabledInOrganization,** операция позволит получить сведения для всех `true` пользователей организации. 

## <a name="example"></a>Пример 

### <a name="request"></a>Запрос

Вот пример запроса на то, как администратор обновляет параметр конфиденциальности **"disabledForGroup",** чтобы запретить отображать сведения о элементах пользователей определенной группы Azure AD.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_iteminsightssettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
Content-type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-iteminsightssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-iteminsightssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-iteminsightssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-iteminsightssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "update_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```


