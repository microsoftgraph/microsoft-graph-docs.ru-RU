---
title: Тип ресурса crossTenantAccessPolicy
description: Межтенантная политика доступа представляет базовую политику в каталоге для параметров межтенантного доступа.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2fb0f51f661938a3ee25edb4519fd5e8bc16987b
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604756"
---
# <a name="crosstenantaccesspolicy-resource-type"></a>Тип ресурса crossTenantAccessPolicy

Пространство имен: microsoft.graph

Представляет базовую политику в каталоге для параметров межтенантного доступа.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Чтение свойств и связей объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|
|[Обновление crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Обновление свойств объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| displayName | Строка | Отображаемое имя политики межтенантного доступа. Наследуется [от policyBase](../resources/policybase.md).|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|default|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Определяет конфигурацию по умолчанию для взаимодействия организации с внешними организациями Azure Active Directory.|
|Партнеров|[Коллекция crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)|Определяет конфигурации, относящиеся к партнерам, для внешних организаций Azure Active Directory.|

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
  "displayName": "String"
}
```
