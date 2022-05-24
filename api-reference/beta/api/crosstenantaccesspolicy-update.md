---
title: Обновление crossTenantAccessPolicy
description: Обновление свойств политики межтенантного доступа.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8b94ab5f20642ea7283d5a3c3552a4b2a271c2e3
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653520"
---
# <a name="update-crosstenantaccesspolicy"></a>Обновление crossTenantAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств политики [межтенантного доступа](../resources/crosstenantaccesspolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.CrossTenantAccess|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Приложение|Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/crossTenantAccessPolicy
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
|displayName|Строка|Отображаемое имя политики межтенантного доступа.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`.

Размер [объекта crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) в настоящее время ограничен 25 КБ. Этот метод возвращает код ошибки `400 Bad Request` , если размер политики превысит 25 КБ.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy
Content-Type: application/json

{
  "allowedCloudEndpoints": ["microsoftonline.us", "partner.microsoftonline.cn"]
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
