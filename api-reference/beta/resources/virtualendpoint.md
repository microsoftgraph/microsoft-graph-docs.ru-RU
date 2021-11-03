---
title: тип ресурса virtualEndpoint
description: Ресурс virtualEndpoint представляет собой контейнер для функций управления облачными ПК.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0c271bbbbe37fe35e6d6a21ec5a232ca5f78a9f2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694868"
---
# <a name="virtualendpoint-resource-type"></a>тип ресурса virtualEndpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для API для управления облачным компьютером.

Используйте API облачного ПК для обеспечения и управления виртуальными рабочими столами для сотрудников организации. Используйте его совместно с [API Intune](../resources/intune-graph-overview.md) для управления физическими и виртуальными конечными точками.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить эффективные разрешения](../api/virtualendpoint-geteffectivepermissions.md)|Коллекция строк|Просмотр эффективных разрешений пользователя, который в настоящее время проходит проверку подлинности.|
|[CloudPCs списка](../api/virtualendpoint-list-cloudpcs.md)|[коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)|
|[Список устройствImages](../api/virtualendpoint-list-deviceimages.md)|[коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Создание cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Создайте новый [объект cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание нового [объекта cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Список provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Создание cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Создайте новый [объект cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Список userSettings](../api/virtualendpoint-list-usersettings.md)|[коллекция cloudPcUserSetting](../resources/cloudpcusersetting.md)|Получите ресурсы cloudPcUserSetting из свойства навигации userSettings.|
|[Создание cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Создание нового объекта cloudPcUserSetting.|
|[Список объектов auditEvent](../api/virtualendpoint-list-auditevents.md)|[коллекция cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Список свойств и связей объектов [cloudPcAuditEvent.](../resources/cloudpcauditevent.md)|
|[Список, поддерживаемыйРегионами](../api/virtualendpoint-list-supportedregions.md)|[коллекция cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Список свойств и связей объектов [cloudPcSupportedRegion.](../resources/cloudpcsupportedregion.md)|
|[Список servicePlans](../api/virtualendpoint-list-serviceplans.md)|[коллекция cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Список свойств и связей объектов [cloudPcServicePlan.](../resources/cloudpcserviceplan.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для идентификатора виртуальной конечной точки. Только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|cloudPCs|[коллекция cloudPC](../resources/cloudpc.md)|Облачные управляемые виртуальные настольные компьютеры.|
|deviceImages|[коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Ресурс изображений на облачном компьютере.|
|onPremisesConnections|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.|
|provisioningPolicies|[коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Политика обеспечения облачного компьютера.|
|userSettings|[коллекция cloudPcUserSetting](../resources/cloudpcusersetting.md)|Параметры пользователей облачного ПК. |
|auditEvents|[коллекция cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Событие аудита облачного компьютера.|
|supportedRegions|[коллекция cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Области, поддерживаемые облачным компьютером.|
|servicePlans|[коллекция cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Планы службы облачных ПК.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
