---
title: Обновление Итеминсигхтс
description: Обновление свойств объекта Итеминсигхтссеттингс
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: a4072a084b632389296266e54e4c0540da69e8ad
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509656"
---
# <a name="update-iteminsightssettings"></a>Обновление Итеминсигхтссеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств указанного ресурса [итеминсигхтссеттингс](../resources/iteminsightssettings.md) .

Сведения о том, как настроить конфиденциальность сведений об элементах для вашей организации, можно узнать в разделе [Настройка конфиденциальности Insights](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0). 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.ReadWrite |

>**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль глобального администратора.

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

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Логический| `true`, если аналитика элемента организации включена; `false`Если аналитика элемента Организации отключена для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательное свойство.|
|disabledForGroup|Строка| Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники". Значение по умолчанию: `empty`. Необязательный параметр.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итеминсигхтссеттингс](../resources/iteminsightssettings.md) в тексте отклика.

>**Примечание:** Эта операция проверяет допустимость значений свойств указанного ресурса **итеминсигхтссеттингс** . Если задано свойство **дисабледфорграуп** , эта операция не проверяет существование соответствующей группы Azure AD. Это означает, что если вы настроили **дисабледфорграуп** для группы Azure AD, которая не существовала или была удалена, то эта операция не сможет определить членство в группах и отключить сведения об элементе для определенных пользователей. Если для параметра **исенаблединорганизатион** задано значение `true` , операция позволит получить информацию для всех пользователей в Организации. 

## <a name="example"></a>Пример 

### <a name="request"></a>Запрос

Ниже приведен пример запроса на изменение параметров конфиденциальности "**дисабледфорграуп**" для администраторов, чтобы запретить отображение элемента для определенной группы Azure AD.

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

---


##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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
