---
title: Обновление crossTenantAccessPolicyConfigurationPartner
description: 'Обновление свойств конфигурации, определенной для партнеров.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="update-crosstenantaccesspolicyconfigurationpartner"></a>Обновление crossTenantAccessPolicyConfigurationPartner

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств конфигурации [, определенной для партнеров](../resources/crosstenantaccesspolicyconfigurationpartner.md) .

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
PATCH /policies/crossTenantAccessPolicy/partners/{id}
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
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров для пользователей из других организаций, имеющих доступ к вашим ресурсам с помощью совместной работы Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию вашего партнера для пользователей в организации, исходящие для доступа к ресурсам в другой организации с помощью совместной работы Azure AD B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию вашего партнера для пользователей из других организаций, имеющих доступ к вашим ресурсам с помощью прямого подключения Azure AD B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию конкретного партнера для пользователей в организации, исходящие для доступа к ресурсам другой организации с помощью прямого подключения Azure AD B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию, определенную для партнеров, для доверия к другим утверждениям условного доступа от внешних Azure Active Directory организаций Azure AD. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners/90e29127-71ad-49c7-9ce8-db3f41ea06f1
Content-Type: application/json

{
  "inboundTrust": 
  {
    "isMfaAccepted": true,
    "isCompliantDeviceAccepted": true,
    "isHybridAzureADJoinedDeviceAccepted" : true
  }
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
