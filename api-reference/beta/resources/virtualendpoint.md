---
title: Тип ресурса Виртуалендпоинт
description: Ресурс Виртуалендпоинт представляет контейнер для функций управления Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 168a6f35a3d758911913422f96ea5dc070d57a47
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378533"
---
# <a name="virtualendpoint-resource-type"></a>Тип ресурса Виртуалендпоинт

Пространство имен: microsoft.graph

Ресурс Виртуалендпоинт представляет контейнер для API для управления облачным компьютером.

Использование API Cloud PC для подготовки виртуальных рабочих столов для сотрудников Организации и управления ими. Используйте его совместно с [API Intune](../resources/intune-graph-overview.md) для управления физическими и виртуальными конечными точками.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение действующих разрешений](../api/virtualendpoint-geteffectivepermissions.md)|Коллекция String|Просмотр действующих разрешений текущего пользователя, прошедшего проверку подлинности.|
|[Список Клаудпкс](../api/virtualendpoint-list-cloudpcs.md)|Коллекция [клаудпк](../resources/cloudpc.md)|Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .|
|[Список Девицеимажес](../api/virtualendpoint-list-deviceimages.md)|Коллекция [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)|Перечисление свойств и связей объектов [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .|
|[Создание Клаудпкдевицеимаже](../api/virtualendpoint-post-deviceimages.md)|[клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)|Создание нового объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .|
|[Список Онпремисесконнектионс](../api/virtualendpoint-list-onpremisesconnections.md)|Коллекция [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Список свойств и связей объектов [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .|
|[Создание Клаудпконпремисесконнектион](../api/virtualendpoint-post-onpremisesconnections.md)|[клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Создание нового объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .|
|[Список ПровисионингполиЦиес](../api/virtualendpoint-list-provisioningpolicies.md)|Коллекция [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|Список свойств и связей объектов [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|
|[Создание Клаудпкпровисионингполици](../api/virtualendpoint-post-provisioningpolicies.md)|[клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|Создание нового объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор идентификатора виртуальной конечной точки. только для чтения.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|клаудпкс|Коллекция [клаудпк](../resources/cloudpc.md)|Облачные управляемые виртуальные рабочие столы.|
|девицеимажес|Коллекция [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)|Ресурс Image (изображение) на облачном компьютере.|
|онпремисесконнектионс|Коллекция [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)|Определенная коллекция сведений о ресурсах Azure, которую можно использовать для установки локальной сети для облачных компьютеров.|
|провисионингполиЦиес|Коллекция [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)|политика подготовки облачных ПК.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
