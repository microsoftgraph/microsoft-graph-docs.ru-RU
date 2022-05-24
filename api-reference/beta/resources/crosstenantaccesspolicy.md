---
title: Тип ресурса crossTenantAccessPolicy
description: Межтенантная политика доступа представляет базовую политику в каталоге для параметров межтенантного доступа.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: beea220ebf3a0b12e40e56997c236b82fcb5d2fe
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653541"
---
# <a name="crosstenantaccesspolicy-resource-type"></a>Тип ресурса crossTenantAccessPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовую политику в каталоге для параметров межтенантного доступа.

Наследуется [от tenantRelationshipAccessPolicyBase](../resources/tenantrelationshipaccesspolicybase.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Чтение свойств и связей объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|
|[Обновление crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|Обновление свойств объекта [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
| displayName | Строка | Отображаемое имя политики межтенантного доступа. Наследуется [от policyBase](../resources/policybase.md).|
| allowedCloudEndpoints | Коллекция строк | Используется для указания облаков Майкрософт, с которыми организация будет сотрудничать. По умолчанию это значение пусто. Поддерживаемые значения для этого поля: `microsoftonline.com`, и `microsoftonline.us``partner.microsoftonline.cn`. |
| определение (не рекомендуется) | Строка | Необработанные определения JSON политики межтенантного доступа. **Устарело. Не используйте.**|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|default|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|Определяет конфигурацию по умолчанию для взаимодействия организации с внешними Azure Active Directory организациями.|
|Партнеров|[Коллекция crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md)|Определяет конфигурации, относящиеся к партнерам, для внешних Azure Active Directory организаций.|

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
  "definition": "String",
  "allowedCloudEndpoints": ["String"]
}
```
