---
title: Тип ресурса cloudPcProvisioningPolicy
description: Представляет политику подготовки облачных компьютеров.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5c9e851bf2a8723507e1eaa84bc014a715908770
ms.sourcegitcommit: da9079132db3261aed80e6fc4b9314d16e0847b3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2022
ms.locfileid: "66186941"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>Тип ресурса cloudPcProvisioningPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику подготовки облачных компьютеров.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Получение cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Чтение свойств и связей объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Создание cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Создайте объект [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Обновление cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Обновление свойств объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Удаление cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|Отсутствует|Удаление объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Назначение cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|Отсутствует |[Назначьте cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) группам пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|alternateResourceUrl|String|URL-адрес альтернативного ресурса, который ссылается на эту политику подготовки. Только для чтения.|
|cloudPcGroupDisplayName|String|Отображаемое имя группы облачных компьютеров, в которой находятся облачные компьютеры. Только для чтения.|
|description|String|Описание политики подготовки.|
|displayName|String|Отображаемое имя политики подготовки.|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|Указывает, как облачные компьютеры будут присоединяться к Azure Active Directory.|
|gracePeriodInHours|Int32|Количество часов ожидания перед повторной подготовкой или отменой подготовки. Только для чтения.|
|id|String|Уникальный идентификатор политики подготовки облачных компьютеров. Только для чтения.|
|imageDisplayName|String|Отображаемое имя подготавливаемого образа ОС.|
|imageId|String|Идентификатор образа ОС, который требуется подготовить на облачных компьютерах. Формат образа типа коллекции: {publisher_offer_sku}. Поддерживаемые значения для каждого из параметров:<ul><li>publisher: Microsoftwindowsdesktop.</li> <li>предложение: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-m365 и 19h2-ent-cpc-os.</li></ul>|
|imageType|CloudPcProvisioningPolicyImageType|Тип образа ОС (настраиваемого или коллекции), который требуется подготовить на облачных компьютерах. Возможные значения: `gallery`, `custom`.|
|localAdminEnabled|Boolean|Указывает, включен ли параметр локального администратора. Если параметр локального администратора включен, конечный пользователь может быть администратором устройства Облачного компьютера. Только для чтения.|
|Managedby|[cloudPcManagementService](../resources/cloudpconpremisesconnection.md#cloudpcmanagementservice-values)|Указывает, какие службы управляют сетевым подключением Azure. Возможные значения: `windows365`, `devBox`, `unknownFutureValue`. Только для чтения.|
|microsoftManagedDesktop|[microsoftManagedDesktop](../resources/microsoftManagedDesktop.md)|Конкретные параметры для Microsoft Managed Desktop, которые позволяют клиентам получить интерфейс управляемого устройства для облачного компьютера. Прежде чем включить Microsoft Managed Desktop, администратор должен настроить его.|
|onPremisesConnectionId|String|Идентификатор cloudPcOnPremisesConnection. Чтобы убедиться, что облачные компьютеры имеют сетевое подключение и присоединены к домену, выберите подключение к виртуальной сети, проверенной службой облачных компьютеров.|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Конкретные Windows настройки при создании облачных компьютеров для этой политики подготовки.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[Коллекция cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md)|Определенная коллекция назначений политик подготовки. Представляет набор групп Microsoft 365 и групп безопасности в Azure AD, для которых назначена политика подготовки. Возвращается только на `$expand`. См [. пример](../api/cloudpcprovisioningpolicy-get.md) получения связи назначений. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "alternateResourceUrl": "String",
  "cloudPcGroupDisplayName": "String",
  "description": "String",
  "displayName": "String",
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  },
  "gracePeriodInHours": "Integer",
  "id": "String (identifier)",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "localAdminEnabled": "Boolean",
  "managedBy": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "onPremisesConnectionId": "String",
  "windowsSettings": {
    "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
  }
}
```
