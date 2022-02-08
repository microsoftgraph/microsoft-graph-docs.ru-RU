---
title: Создание crossTenantAccessPolicyConfigurationPartner
description: Создайте новую конфигурацию партнеров в политике доступа между клиентами.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="create-crosstenantaccesspolicyconfigurationpartner"></a>Создание crossTenantAccessPolicyConfigurationPartner

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новую конфигурацию партнеров в политике доступа между клиентами.

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
POST /policies/crossTenantAccessPolicy/partners
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляют представление JSON объекта [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) .

В следующей таблице показаны свойства, необходимые при создании [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию для партнеров для пользователей из других организаций, имеющих доступ к вашим ресурсам с помощью совместной работы Azure AD B2B. |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию вашего партнера для пользователей в организации, исходящие для доступа к ресурсам в другой организации с помощью совместной работы Azure AD B2B. |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию вашего партнера для пользователей из других организаций, имеющих доступ к вашим ресурсам с помощью прямого подключения Azure AD B2B. |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию конкретного партнера для пользователей в организации, исходящие для доступа к ресурсам другой организации с помощью прямого подключения Azure AD B2B. |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию для конкретного партнера для доверия к другим утверждениям условного доступа от внешних организаций Azure AD. |
| tenantId | String | Идентификатор клиента для организации Azure Active Directory (Azure AD). |

## <a name="response"></a>Отклик

В случае успешной `201 Created` работы этот метод возвращает код ответа и [объект crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_crosstenantaccesspolicyconfigurationpartner_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners
Content-Type: application/json

{
  "tenantId": "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a",
  "b2bDirectConnectOutbound": 
  {
    "usersAndGroups": 
    {
      "accessType": "blocked",
      "targets": [
        {
            "target": "6f546279-4da5-4b53-a095-09ea0cef9971",
            "targetType": "group"
        }
      ]
    }
  },
  "b2bDirectConnectInbound": 
  {
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

### <a name="response"></a>Ответ

Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "tenantId": "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a",
  "inboundTrust": null,
  "b2bCollaborationInbound": null,
  "b2bCollaborationOutbound": null,
  "b2bDirectConnectOutbound": 
  {
    "usersAndGroups":
    {
      "accessType": "blocked",
      "targets": [
        {
          "target": "6f546279-4da5-4b53-a095-09ea0cef9971",
          "targetType": "group"
        }
      ]
    }
  },
  "b2bDirectConnectInbound":
  {
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
