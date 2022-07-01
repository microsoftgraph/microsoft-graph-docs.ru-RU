---
title: Тип ресурса crossTenantAccessPolicyInboundTrust
description: Определяет утверждения условного доступа, которые вы хотите принять от других организаций с помощью конфигурации политики межтенантного доступа.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fef57d6a1ae940677d7d5412838223618d9aae66
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604744"
---
# <a name="crosstenantaccesspolicyinboundtrust-resource-type"></a>Тип ресурса crossTenantAccessPolicyInboundTrust

Пространство имен: microsoft.graph

Определяет утверждения условного доступа, которые вы хотите принять из других Azure AD с помощью конфигурации политики межтенантного доступа. Их можно настроить в конфигурации по умолчанию, конфигурации для конкретного партнера или в обоих вариантах.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| isCompliantDeviceAccepted | Boolean | Указывает, являются ли совместимые устройства из внешних Azure AD доверенными. |
| isHybridAzureADJoinedDeviceAccepted | Boolean | Указывает, являются ли Azure AD присоединенные к гибридной среде устройства из внешних Azure AD доверенными. |
| isMfaAccepted | Boolean | Указывает, является ли многофакторная проверка подлинности из внешних Azure AD доверенными организациями.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
