---
title: 'пользователь: активироватьServicePlan'
description: Активация плана службы с `servicePlanId` заданным и для данного `skuId` пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 70849865237a82f4a0bb5fcee22263291627c21d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578868"
---
# <a name="user-activateserviceplan"></a>пользователь: активироватьServicePlan

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Активация плана службы с `servicePlanId` заданным и для данного `skuId` пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
| :--- | :--- |
| Делегированные (рабочая или учебная учетная запись) | Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /users/{id | userPrincipalName}/activateServicePlan
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
| :--- | :--- |
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса укажи объект JSON со следующим параметром:

| Параметр | Тип | Описание |
| :--- | :--- | :--- |
| servicePlanId | Guid | PlanId servicePlan для активации. |
| skuId | Guid | SkuId SKU, в планах службы. |

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "user_activateserviceplan"
}
-->

``` http
POST https://graph.microsoft.com/beta/me/activateServicePlan
Content-type: application/json
Content-length: 115

{
  "servicePlanId": "28f42d6f-8034-4a0f-9d8a-a218a63b3299",
  "skuId": "465a2a90-5e59-456d-a7b8-127b9fb2e484"
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
