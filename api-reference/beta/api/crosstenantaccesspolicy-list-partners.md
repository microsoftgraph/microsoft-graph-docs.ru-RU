---
title: Партнеры списка
description: Получите список всех конфигураций партнеров в рамках политики меж клиента доступа.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="list-partners"></a>Партнеры списка

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список всех конфигураций партнеров в рамках политики меж клиента доступа.

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
GET /policies/crossTenantAccessPolicy/partners
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успеха `200 OK` этот метод возвращает код отклика и коллекцию объектов [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "list_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.crossTenantAccessPolicyConfigurationPartner)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "tenantId": "123f4846-ba00-4fd7-ba43-dac1f8f63013",
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
  ]
}
```
