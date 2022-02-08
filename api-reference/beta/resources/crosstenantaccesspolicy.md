---
title: тип ресурса crossTenantAccessPolicy
description: Политика доступа между клиентами представляет базовую политику в каталоге для параметров меж клиента.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicy-resource-type"></a>тип ресурса crossTenantAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовую политику в каталоге для параметров межъединого доступа.

Наследует от [tenantRelationshipAccessPolicyBase](../resources/tenantrelationshipaccesspolicybase.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|
|[Обновление crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Обновление свойств объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| displayName | Строка | Отображает имя политики меж клиента доступа. Унаследовано от [policyBase](../resources/policybase.md).|
| lastModifiedDateTime | DateTimeOffset | Время последнего изменения политики доступа к клиенту с использованием формата ISO 8601 и всегда во время UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| определение (неподготовленное) | String | Необработанные определения JSON политики меж клиента доступа. **Устарело. Не используйте.**|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|default|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Определяет конфигурацию по умолчанию для взаимодействия организации с внешними Azure Active Directory организациями.|
|партнеры|[коллекция crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)|Определяет конфигурации для внешних Azure Active Directory партнеров.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicy",
  "baseType": "microsoft.graph.tenantRelationshipAccessPolicyBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicy",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "definition": "String"
}
```
