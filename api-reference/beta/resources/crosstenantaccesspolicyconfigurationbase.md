---
title: тип ресурса crossTenantAccessPolicyConfigurationBase
description: 'Определяет свойства, распространенные в конфигурации политики доступа между клиентом для параметров по умолчанию и для партнеров.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyconfigurationbase-resource-type"></a>тип ресурса crossTenantAccessPolicyConfigurationBase

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, определяя свойства, распространенные в конфигурации политики доступа между клиентами для параметров по умолчанию и для партнеров, управляющих совместной Azure Active Directory (Azure AD) B2B и B2B direct connect.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|b2bCollaborationInbound|[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md)|Определяет конфигурацию для пользователей из других организаций, имеющих доступ к ресурсам с помощью совместной работы Azure AD B2B.|
|b2bCollaborationOutbound|[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md)|Определяет конфигурацию для пользователей в организации, исходящие для доступа к ресурсам в другой организации с помощью совместной работы Azure AD B2B.|
|b2bDirectConnectInbound|[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md)|Определяет конфигурацию для пользователей из других организаций, имеющих доступ к ресурсам с помощью прямого подключения Azure AD B2B.|
|b2bDirectConnectOutbound|[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md)|Определяет конфигурацию для пользователей в организации, исходящие для доступа к ресурсам другой организации с помощью прямого подключения Azure AD B2B.|
|inboundTrust|[crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md)|Определяет конфигурацию для доверия к другим утверждениям условного доступа от внешних организаций Azure AD.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationBase",
  "inboundTrust": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
  },
  "b2bCollaborationOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bCollaborationInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  }
}
```
