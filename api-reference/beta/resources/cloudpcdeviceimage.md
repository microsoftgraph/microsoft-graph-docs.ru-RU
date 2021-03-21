---
title: тип ресурса cloudPcDeviceImage
description: Представляет ресурс изображений на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d4a88bb4d826ead30d1d739e696dec76df5cbb2f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957067"
---
# <a name="cloudpcdeviceimage-resource-type"></a>тип ресурса cloudPcDeviceImage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс изображений на облачном компьютере.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список устройствImages](../api/virtualendpoint-list-deviceimages.md)|[коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Get cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Создание cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Создайте новый [объект cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Удаление cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|Нет|Удаление [объекта cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[коллекция cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)|Получите [объекты cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для ресурса изображений на облачном компьютере. Только для чтения.|
|sourceImageResourceId|Строка|ID источника ресурса изображений в Azure. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|displayName|Строка|Имя отображения изображения.|
|version|String|Версия изображения. Например: 0.0.1, 1.5.13.|
|osBuildNumber|Строка|Версия сборки ОС изображения. Например: 1909.|
|operatingSystem|String|Операционная система изображения. Например: Windows 10 Enterprise.|
|lastModifiedDateTime|DateTimeOffset|Данные и время последнего изменения изображения. Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'.|
|status|cloudPcDeviceImageStatus|Состояние изображения на облачном компьютере. Возможные значения: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Сведения о состоянии изображения, который указывает, почему не удалось загрузить, если применимо. Возможные значения: `internalServerError`, `sourceImageNotFound`.|

### <a name="cloudpcdeviceimagestatus-values"></a>значения cloudPcDeviceImageStatus

|Member|Описание|
|:---|:---|
|ожидание|Загрузка изображения продолжается.|
|готово|Изображение готово для использования на облачных ПК.|
|не удалось|Изображение не может быть загружено. |

### <a name="cloudpcdeviceimagestatusdetails-values"></a>значения cloudPcDeviceImageStatusDetails

|Member|Описание|
|:---|:---|
|internalServerError|При обработке изображения произошла внутренняя ошибка сервера.|
|sourceImageNotFound|Исходный образ недоступен или не найден.|
|osVersionNotSupported| Версия ОС не поддерживается.|
|sourceImageInvalid|Исходный образ не является допустимым для обеспечения windows VM с ним.|

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
