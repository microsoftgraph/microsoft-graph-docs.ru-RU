---
title: тип ресурса crossTenantAccessPolicyConfigurationDefault
description: 'Конфигурация по умолчанию, определяемая для входящие и исходящие параметры совместной работы Azure AD B2B и прямого подключения B2B.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyconfigurationdefault-resource-type"></a>тип ресурса crossTenantAccessPolicyConfigurationDefault

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Конфигурация по умолчанию, определяемая для входящие и исходящие параметры совместной работы Azure AD B2B и прямого подключения B2B.

Наследуется [от crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md)|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Получите конфигурацию по умолчанию для B2B-совместной работы и параметров прямого подключения B2B к входящие и исходящие.|
|[Обновление crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-update.md)|Нет|Обновление конфигурации по умолчанию для B2B-совместной работы и параметров прямого подключения B2B.|
|[Сброс по умолчанию системы](../api/crosstenantaccesspolicyconfigurationdefault-resettosystemdefault.md)|Нет|Сброс конфигурации по умолчанию для политики межзаявного доступа к параметрам по умолчанию системы.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей из других организаций, имеющих доступ к ресурсам с помощью совместной работы Azure AD B2B. Наследуется [от crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей в организации, исходящие для доступа к ресурсам в другой организации с помощью совместной работы Azure AD B2B. Наследуется [от crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bDirectConnectInbound  |[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | Определяет конфигурацию по умолчанию для пользователей из других организаций, имеющих доступ к ресурсам с помощью прямого подключения Azure AD B2B. Наследуется [от crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |Определяет конфигурацию по умолчанию для пользователей в организации, исходящие для доступа к ресурсам другой организации с помощью прямого подключения Azure AD B2B. Наследуется [от crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | Определяет конфигурацию по умолчанию для доверия к другим утверждениям условного доступа от внешних организаций Azure AD. Наследуется [от crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md). |
| isServiceDefault | Логический | Если `true`конфигурация по умолчанию установлена для конфигурации системы по умолчанию. Если `false`параметры по умолчанию настроены. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
  "baseType": "microsoft.graph.crossTenantAccessPolicyConfigurationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
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
  },
  "isServiceDefault": "Boolean"
}
```
