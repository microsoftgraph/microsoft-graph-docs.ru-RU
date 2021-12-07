---
title: Сведения об обновлении
description: Обновление свойств объекта insightsSettings
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 7af541c033cebb9409ac1bf61a8470b1c67726a0
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322787"
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

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` если для организации включен указанный тип анализа; если указанный тип анализа отключен для `false` всех пользователей без исключений. Значение по умолчанию: `true`. Необязательно.|
|disabledForGroup|String| ID группы Azure AD, в которой указанный тип данных отключен для ее участников. Значение по умолчанию: `empty`. Необязательно.|

>**Примечание:** Эта операция не проверяет значение **свойства disabledForGroup,** если оно включено в тело запроса. Если задайте **свойство disabledForGroup** строке, эта операция не проверяет наличие соответствующей группы Azure AD. Это означает, что если вы установите **disabledForGroup** в группу Azure AD, которая не существует или удаляется после этого, эта операция не сможет идентифицировать членство в группе и отключить сведения о элементе или пользователях для определенных пользователей. Если **установлено isEnabledInOrganization,** операция позволит получить указанный тип данных для всех пользователей `true` организации.  
## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект insightsSettings](../resources/insightssettings.md) в тексте ответа.

## <a name="examples"></a>Примеры 

### <a name="example-1-update-settings-for-item-insights"></a>Пример 1. Обновление параметров для анализа элементов
#### <a name="request"></a>Запрос

Вот пример запроса, который показывает, как администратор обновляет параметр конфиденциальности **"disabledForGroup",** чтобы запретить отображать сведения о элементах пользователей в определенной группе Azure AD.


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
