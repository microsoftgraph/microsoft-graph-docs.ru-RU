---
title: Тип ресурса virtualEndpoint
description: Ресурс virtualEndpoint представляет контейнер для функций управления облачными КОМПЬЮТЕРами.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ea76f9267bc9be33c88a4d6a615f2fe881a3b193
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156681"
---
# <a name="virtualendpoint-resource-type"></a>Тип ресурса virtualEndpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс virtualEndpoint представляет контейнер для API для управления облачным компьютером.

Используйте API облачных КОМПЬЮТЕРов для предоставления и управления виртуальными рабочими столами для сотрудников организации. Используйте его вместе с [API Intune](../resources/intune-graph-overview.md) для управления физическими и виртуальными конечными точками.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получите эффективные разрешения](../api/virtualendpoint-geteffectivepermissions.md)|Коллекция String|Просмотр эффективных разрешений для пользователя, который в настоящее время проходит проверку подлинности.|
|[Список cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[Коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)|
|[Список deviceImages](../api/virtualendpoint-list-deviceimages.md)|[Коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Создание cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Создание объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Список onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[Коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Создание cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Создание объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)|
|[Список provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[Коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|
|[Создание cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|Создание объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для идентификатора виртуальной конечной точки. Только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|cloudPCs|[Коллекция cloudPC](../resources/cloudpc.md)|Виртуальные рабочие столы, управляемые облаком.|
|deviceImages|[Коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Ресурс изображения на облачном компьютере.|
|onPremisesConnections|[Коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|Заданная коллекция сведений о ресурсах Azure, которую можно использовать для подключения к локальной сети для облачных компьютеров.|
|provisioningPolicies|[Коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|политика предоставления облачных компьютеров;|

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
