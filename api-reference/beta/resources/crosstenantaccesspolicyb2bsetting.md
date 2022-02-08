---
title: тип ресурса crossTenantAccessPolicyB2BSetting
description: Определяет входящие и исходящие правила для совместной Azure Active Directory (Azure AD) B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyb2bsetting-resource-type"></a>тип ресурса crossTenantAccessPolicyB2BSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет входящие и исходящие правила для совместной Azure Active Directory (Azure AD) B2B.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|приложения|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|Список приложений, целевых с помощью политики меж клиента доступа.|
|usersAndGroups|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|Список пользователей и групп, на которые ориентирована политика межсетевого доступа.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyB2BSetting",
  "usersAndGroups": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
  },
  "applications": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
  }
}
```
