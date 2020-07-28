---
title: Получение Итеминсигхтс
description: Получение свойств объекта Итеминсигхтссеттингс
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: cc081f9d1fc34f1935f788cf936e376a647cdf7d
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427553"
---
# <a name="get-iteminsightssettings"></a>Получение Итеминсигхтссеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств объекта [итеминсигхтссеттингс](../resources/iteminsightssettings.md) .

Сведения о том, как настроить конфиденциальность сведений об элементах для вашей организации, можно узнать в разделе [Настройка конфиденциальности Insights](/graph/insights-customize-item-insights-privacy.md). 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | User.Read, User.ReadWrite |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read, User.ReadWrite  |

>**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль глобального администратора.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

```http
GET /organization/{organizationId}/settings/itemInsights
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [итеминсигхтссеттингс](../resources/iteminsightssettings.md) в тексте отклика.

>**Примечание:** Эта операция проверяет допустимость значений свойств указанного ресурса **итеминсигхтссеттингс** . Если задано свойство **дисабледфорграуп** , эта операция не проверяет существование соответствующей группы Azure AD. Это означает, что если вы настроили **дисабледфорграуп** для группы Azure AD, которая не существовала или была удалена, то эта операция не сможет определить членство в группах и отключить сведения об элементе для определенных пользователей. Если для параметра **исенаблединорганизатион** задано значение `true` , операция позволит получить информацию для всех пользователей в Организации. 

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_iteminsightssettings"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{organizationId}/settings/itemInsights
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. 
> **Примечание.** Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemInsightsSettings",
  "name": "get_iteminsightssettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isEnabledInOrganization": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
