---
title: тип ресурса cloudPcDeviceImage
description: Представляет ресурс изображений на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 2c38895059461f814a3ad0f8e663082972cc8663
ms.sourcegitcommit: e96b98849cfc3aa915df63696a0b9f30c0a52cfd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2021
ms.locfileid: "51654130"
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
|id|String|Уникальный идентификатор для ресурса изображений на облачном компьютере. Только для чтения.|
|sourceImageResourceId|String|ID источника ресурса изображений в Azure. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|displayName|String|Имя отображения изображения.|
|version|String|Версия изображения. Например: 0.0.1, 1.5.13.|
|osBuildNumber|String|Версия сборки ОС изображения. Например: 1909.|
|operatingSystem|String|Операционная система изображения. Например: Windows 10 Enterprise.|
|lastModifiedDateTime|DateTimeOffset|Данные и время последнего изменения изображения. Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'.|
|status|cloudPcDeviceImageStatus|Состояние изображения на облачном компьютере. Возможные значения: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Сведения о состоянии изображения, который указывает, почему не удалось загрузить, если применимо. Возможные значения: `internalServerError` , , и `sourceImageNotFound` `osVersionNotSupported` `sourceImageInvalid` .|

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
