---
title: тип ресурса managementActionTenantDeploymentStatus
description: Представляет состояние развертывания уровня клиента для действия управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 1967c3ad96cc9c4e76a718cafab7ba14207753a9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402711"
---
# <a name="managementactiontenantdeploymentstatus-resource-type"></a>тип ресурса managementActionTenantDeploymentStatus

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние развертывания уровня клиента для действия управления.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Управление спискамиActionTenantDeploymentStatus](../api/managedtenants-managedtenant-list-managementactiontenantdeploymentstatuses.md)|[коллекция microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|Получите список объектов [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) и их свойств.|
|[Get managementActionTenantDeploymentStatus](../api/managedtenants-managementactiontenantdeploymentstatus-get.md)|[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|Ознакомьтесь с свойствами и отношениями объекта [managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|
|[changeDeploymentStatus](../api/managedtenants-managementactiontenantdeploymentstatus-changedeploymentstatus.md)|[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|Изменение состояния развертывания для действия управления.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор состояния развертывания уровня клиента. Обязательный. Только для чтения.|
|состояния|[коллекция microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)|Набор состояния развертывания для каждого экземпляра действия управления. Необязательное.|
|tenantGroupId|String|Идентификатор группы клиента, связанной с действием управления. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "id": "String (identifier)",
  "tenantGroupId": "String",
  "tenantId": "String",
  "statuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
    }
  ]
}
```
