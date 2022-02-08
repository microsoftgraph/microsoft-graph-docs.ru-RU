---
title: тип ресурса crossTenantAccessPolicyInboundTrust
description: 'Определяет утверждения условного доступа, которые вы хотите принять от других организаций с помощью конфигурации политики межзаймного доступа.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyinboundtrust-resource-type"></a>тип ресурса crossTenantAccessPolicyInboundTrust

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет утверждения условного доступа, которые необходимо принять из других организаций Azure AD с помощью конфигурации политики межзаявного доступа. Они могут быть настроены в конфигурации по умолчанию, конфигурации, определенной для партнеров, или в обоих.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| isCompliantDeviceAccepted | Логический | Указывает, доверять ли совместимым устройствам из внешних организаций Azure AD. |
| isHybridAzureADJoinedDeviceAccepted | Логический | Указывает, являются ли доверенными гибридные устройства Azure AD из внешних организаций Azure AD. |
| isMfaAccepted | Логический | Указывает, доверяется ли MFA из внешних организаций Azure AD.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyInboundTrust",
  "isMfaAccepted": "Boolean",
  "isCompliantDeviceAccepted": "Boolean",
  "isHybridAzureADJoinedDeviceAccepted": "Boolean"
}
```
