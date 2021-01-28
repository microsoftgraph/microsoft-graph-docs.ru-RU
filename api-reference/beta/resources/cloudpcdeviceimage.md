---
title: Тип ресурса cloudPcDeviceImage
description: Представляет ресурс изображения на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 14e3f28d9e7d91df953405bc36afff4d3405c886
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033901"
---
# <a name="cloudpcdeviceimage-resource-type"></a>Тип ресурса cloudPcDeviceImage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс изображения на облачном компьютере.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список deviceImages](../api/virtualendpoint-list-deviceimages.md)|[Коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Get cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Чтение свойств и связей объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Создание cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Создание объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Удаление cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|Нет|Удаление объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[Коллекция cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)|Получите [объекты cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор ресурса изображения на облачном компьютере. Только для чтения.|
|sourceImageResourceId|String|ИД ресурса исходных изображений в Azure. Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|displayName|String|Отображаемая фамилия изображения.|
|version|String|Версия изображения. Например: 0.0.1, 1.5.13.|
|osBuildNumber|String|Версия сборки ОС образа. Например: 1909.|
|operatingSystem|String|Операционная система образа. Например: Windows 10 Корпоративная.|
|lastModifiedDateTime|DateTimeOffset|Данные и время последнего изменения изображения. Время отображается в формате ISO 8601 и времени в формате UTC. Например, полночь 1 января 2014 г. в UTC отображается как "2014-01-01T00:00:00Z".|
|status|cloudPcDeviceImageStatus|Состояние изображения на облачном компьютере. Возможные значения: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Сведения о состоянии изображения, которые указывают, почему не удалось отправить, если применимо. Возможные значения: `internalServerError`, `sourceImageNotFound`.|

### <a name="cloudpcdeviceimagestatus-values"></a>Значения cloudPcDeviceImageStatus

|Member|Описание|
|:---|:---|
|pending|Идет отправка изображения.|
|ready|Изображение готово к использованию на облачных ПК.|
|failed|Не удалось отправить изображение. |

### <a name="cloudpcdeviceimagestatusdetails-values"></a>Значения cloudPcDeviceImageStatusDetails

|Member|Описание|
|:---|:---|
|internalServerError|При обработке образа произошла внутренняя ошибка сервера.|
|sourceImageNotFound|Исходный образ не является допустимым для предоставления к ней ВМ Для Windows.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
