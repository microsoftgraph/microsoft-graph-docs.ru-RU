---
title: тип ресурса cloudPcDeviceImage
description: Представляет ресурс изображений на облачном компьютере.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: eb46059f675fc392fe0ec3c83d7c3cb6ba60e869
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567400"
---
# <a name="cloudpcdeviceimage-resource-type"></a>тип ресурса cloudPcDeviceImage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс изображений на облачном компьютере.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список устройствImages](../api/virtualendpoint-list-deviceimages.md)|[коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Get cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Создание cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Создайте новый [объект cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[Удаление cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|Нет|Удаление [объекта cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[коллекция cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)|Получите [объекты cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)|
|[Перезагрузка cloudPcDeviceImage](../api/cloudpcdeviceimage-reupload.md)|Нет|Перезагрузите [объект cloudPcDeviceImage,](../resources/cloudpcdeviceimage.md) который не удалось загрузить.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения изображения.|
|expirationDate|Дата|Дата, когда изображение стало недоступным.|
|id|Строка|Уникальный идентификатор для ресурса изображений на облачном компьютере. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Данные и время последнего изменения изображения. Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'.|
|operatingSystem|String|Операционная система изображения. Например: Windows 10 Корпоративная.|
|osBuildNumber|Строка|Версия сборки ОС изображения. Например: 1909.|
|osStatus|[cloudPcDeviceImageOsStatus](#cloudpcdeviceimageosstatus-values)|Состояние ОС этого изображения. Возможные значения: `supported`, `supportedWithWarning`, `unknownFutureValue`.|
|sourceImageResourceId|Строка|ID источника ресурса изображений в Azure. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|status|[cloudPcDeviceImageStatus](#cloudpcdeviceimagestatus-values)|Состояние изображения на облачном компьютере. Возможные значения: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Сведения о состоянии изображения, который указывает, почему не удалось загрузить, если применимо. Возможные значения: `internalServerError` `sourceImageNotFound` , , , , `osVersionNotSupported` и `sourceImageInvalid` `sourceImageNotGeneralized` .|
|version|String|Версия изображения. Например: 0.0.1, 1.5.13.|

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
|sourceImageInvalid|Исходный образ не является допустимым для Windows VM с ним.|
|sourceImageNotGeneralized|Загруженное изображение не было обобщено. Перезагрузите изображение после запуска команды sysprep/generalize. Дополнительные сведения см. в [примере Remove machine specific information by generalizing a VM before creating an image.](/azure/virtual-machines/generalize)|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

### <a name="cloudpcdeviceimageosstatus-values"></a>значения cloudPcDeviceImageOsStatus

|Member|Описание|
|:---|:---|
|поддерживается|Изображение устройства активно и готово для использования для предварительной проготовки.|
|supportedWithWarning|Срок действия изображения устройства истек, но облачный КОМПЬЮТЕР продолжит поддержку. Если пользователи продолжают использовать, они могут не получать обновления безопасности.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

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
  "sourceImageResourceId": "String",
  "expirationDate":"String (timestamp)",
  "osStatus":"String"
}
```
