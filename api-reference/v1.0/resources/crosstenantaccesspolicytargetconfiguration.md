---
title: Тип ресурса crossTenantAccessPolicyTargetConfiguration
description: Определяет целевой объект конфигурации параметров политики межтенантного доступа.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5480a471a1114da710d9efaa859b7a6fbcb1749f
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604720"
---
# <a name="crosstenantaccesspolicytargetconfiguration-resource-type"></a>Тип ресурса crossTenantAccessPolicyTargetConfiguration

Пространство имен: microsoft.graph

Определяет целевой объект конфигурации параметров политики межтенантного доступа.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| accessType| crossTenantAccessPolicyTargetConfigurationAccessType | Определяет, разрешен или заблокирован доступ. Допустимые значения: `allowed`, `blocked`, `unknownFutureValue`. |
|targets|[Коллекция crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md)|Указывает, следует ли использовать это правило для пользователей, групп или приложений.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyTargetConfiguration",
  "accessType": "String",
  "targets": [
    {
      "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
    }
  ]
}
```
