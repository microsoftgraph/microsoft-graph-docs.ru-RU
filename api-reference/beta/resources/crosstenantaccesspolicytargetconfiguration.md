---
title: тип ресурса crossTenantAccessPolicyTargetConfiguration
description: Определяет цель конфигурации политики параметров доступа между клиентом.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicytargetconfiguration-resource-type"></a>тип ресурса crossTenantAccessPolicyTargetConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет цель конфигурации политики параметров доступа между клиентом.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| accessType| crossTenantAccessPolicyTargetConfigurationAccessType | Определяет, разрешен ли доступ или заблокирован. Допустимые значения: `allowed`, `blocked`, `unknownFutureValue`. |
|targets|[коллекция crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md)|Указывает, следует ли нацелить пользователей, группы или приложения с этим правилом.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
