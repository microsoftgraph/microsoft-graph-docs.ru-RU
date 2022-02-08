---
title: Обновление crossTenantAccessPolicyConfigurationDefault
description: Обновление конфигурации по умолчанию политики доступа между клиентами.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="update-crosstenantaccesspolicyconfigurationdefault"></a>Обновление crossTenantAccessPolicyConfigurationDefault

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление [конфигурации по умолчанию](../resources/crosstenantaccesspolicyconfigurationdefault.md) политики доступа между клиентами.

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
PATCH /policies/crossTenantAccessPolicy/default
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
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию по умолчанию для доверия к другим утверждениям условного доступа от внешних организаций Azure AD. |
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей из других организаций, имеющих доступ к ресурсам с помощью совместной работы Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей в организации, исходящие для доступа к ресурсам в другой организации с помощью совместной работы Azure AD B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей из других организаций, имеющих доступ к ресурсам с помощью прямого подключения Azure AD B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей в организации, исходящие для доступа к ресурсам другой организации с помощью прямого подключения Azure AD B2B. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_crosstenantaccesspolicyconfigurationdefault"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/default
Content-Type: application/json

{
  "b2bCollaborationOutbound":
  {
    "usersAndGroups":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "0be493dc-cb56-4a53-936f-9cf64410b8b0",
          "targetType": "group"
        }
      ]
    },
    "applications":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "AllApplications",
          "targetType": "application"
        }
      ]
    }
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
