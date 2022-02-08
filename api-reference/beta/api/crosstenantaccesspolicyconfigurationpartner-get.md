---
title: Get crossTenantAccessPolicyConfigurationPartner
description: 'Ознакомьтесь с свойствами и отношениями конфигурации, определенной для партнеров.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="get-crosstenantaccesspolicyconfigurationpartner"></a>Get crossTenantAccessPolicyConfigurationPartner

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями конфигурации [, определенной для партнеров](../resources/crosstenantaccesspolicyconfigurationpartner.md) .

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
GET /policies/crossTenantAccessPolicy/partners/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешной `200 OK` работы этот метод возвращает код ответа и [объект crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "tenantId": "9c5d131d-b1c3-4fc4-9e3f-c6557947d551",
  "inboundTrust": null,
  "b2bCollaborationInbound": null,
  "b2bCollaborationOutbound": null,
  "b2bDirectConnectOutbound": null,
  "b2bDirectConnectInbound":
  {
    "usersAndGroups": 
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "AllUsers",
          "targetType": "user"
        }
      ]
    },
    "applications":
    {
      "accessType": "allowed",
      "targets": [
        {
          "target": "Office365",
          "targetType": "application"
        }
      ]
    }
  }
}
```
