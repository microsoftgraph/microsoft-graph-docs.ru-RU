---
title: тип ресурса virtualEndpoint
description: Ресурс virtualEndpoint представляет собой контейнер для функций управления облачными ПК.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c2e31e7561685e8ad1ca7f9b58bbfcd600c3ce78
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878661"
---
# <a name="virtualendpoint-resource-type"></a>тип ресурса virtualEndpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для API для управления облачными компьютерами.

Используйте API облачного ПК для подготовки и управления виртуальными рабочими столами для сотрудников организации или наряду с [API Intune](../resources/intune-graph-overview.md) для управления физическими и виртуальными конечными точками.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить эффективные разрешения](../api/virtualendpoint-geteffectivepermissions.md)|Коллекция строк|Просмотр эффективных разрешений пользователя, который в настоящее время проходит проверку подлинности.|
|[CloudPCs списка](../api/virtualendpoint-list-cloudpcs.md)|[коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC](../resources/cloudpc.md) .|
|[Список устройствImages](../api/virtualendpoint-list-deviceimages.md)|[коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Список свойств и связей объектов [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Списки galleryImages](../api/virtualendpoint-list-galleryimages.md)|[коллекция cloudPcGalleryImage](../resources/cloudpcgalleryimage.md)|Список свойств и связей объектов [cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) .|
|[Создание cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Создайте новый [объект cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание нового [объекта cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .|
|[Список provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Создание cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Создайте новый [объект cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .|
|[Список userSettings](../api/virtualendpoint-list-usersettings.md)|[коллекция cloudPcUserSetting](../resources/cloudpcusersetting.md)|Получите ресурсы cloudPcUserSetting из свойства навигации userSettings.|
|[Создание cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Создание нового объекта cloudPcUserSetting.|
|[Список объектов auditEvent](../api/virtualendpoint-list-auditevents.md)|[коллекция cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Список свойств и связей объектов [cloudPcAuditEvent](../resources/cloudpcauditevent.md) .|
|[Список, поддерживаемыйРегионами](../api/virtualendpoint-list-supportedregions.md)|[коллекция cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Список свойств и связей объектов [cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md) .|
|[Список servicePlans](../api/virtualendpoint-list-serviceplans.md)|[коллекция cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Список свойств и связей объектов [cloudPcServicePlan](../resources/cloudpcserviceplan.md) .|
|[Снимки списка](../api/virtualendpoint-list-snapshots.md)|[коллекция cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Получите список объектов [cloudPcSnapshot](../resources/cloudpcsnapshot.md) и их свойств.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор виртуальной конечной точки. Только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|auditEvents|[коллекция cloudPcAuditEvent](../resources/cloudpcauditevent.md)|Событие аудита облачного компьютера.|
|cloudPCs|[коллекция cloudPC](../resources/cloudpc.md)|Облачные управляемые виртуальные настольные компьютеры.|
|deviceImages|[коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Ресурс изображений на облачном компьютере.|
|galleryImages|[коллекция cloudPcGalleryImage](../resources/cloudpcgalleryimage.md)|Ресурс изображений галереи на облачном компьютере.|
|onPremisesConnections|[коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Определенный набор сведений о ресурсах Azure, которые можно использовать для создания локальной сетевой связи для облачных компьютеров.|
|organisationSettings|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) |Параметры организации облачного ПК для клиента. |
|provisioningPolicies|[коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Политика обеспечения облачного компьютера.|
|servicePlans|[коллекция cloudPcServicePlan](../resources/cloudpcserviceplan.md)|Планы службы облачных ПК.|
|моментальные снимки|[коллекция cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Снимки облачного ПК.|
|supportedRegions|[коллекция cloudPcSupportedRegion](../resources/cloudpcsupportedregion.md)|Области, поддерживаемые облачным компьютером.|
|userSettings|[коллекция cloudPcUserSetting](../resources/cloudpcusersetting.md)|Параметры пользователей облачного ПК. |
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
