---
title: Тип ресурса crossTenantAccessPolicyB2BSetting
description: Определяет наборы правил для входящего и исходящего трафика для совместной работы Azure Active Directory (Azure AD) B2B.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: aa1740e9cde55faa8cac28c270381c3a0eff1739
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604753"
---
# <a name="crosstenantaccesspolicyb2bsetting-resource-type"></a>Тип ресурса crossTenantAccessPolicyB2BSetting

Пространство имен: microsoft.graph

Определяет наборы правил для входящего и исходящего трафика для совместной работы Azure Active Directory (Azure AD) B2B.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|Приложений|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|Список приложений, предназначенных для политики межтенантного доступа.|
|usersAndGroups|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|Список пользователей и групп, предназначенных для политики межтенантного доступа.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
