---
title: Get crossTenantAccessPolicy
description: Ознакомьтесь с свойствами и отношениями объекта crossTenantAccessPolicy.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="get-crosstenantaccesspolicy"></a>Get crossTenantAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.Read.All, Policy.ReadWrite.CrossTenantAccess|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Приложение|Policy.Read.All, Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/crossTenantAccessPolicy
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешной работы этот метод возвращает код `200 OK` отклика и [объект crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_crosstenantaccesspolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy
```

### <a name="response"></a>Ответ

>**Примечание:** Если вы никогда не меняли параметры меж клиента, этот ответ возвращается `{}`.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.crossTenantAccessPolicy",
    "displayName": "CrossTenantAccessPolicy",
    "lastModifiedDateTime": "08-23-2021Z00:00:00",
    "definition": "Cross tenant access policy..."
  }
}
```
