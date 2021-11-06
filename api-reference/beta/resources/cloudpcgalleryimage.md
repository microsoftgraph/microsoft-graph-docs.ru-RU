---
title: тип ресурса cloudPcGalleryImage
description: Представляет ресурс изображений галереи текущей организации.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7c539af9b8a31000af06cb88de594d80c4ea5eb5
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805564"
---
# <a name="cloudpcgalleryimage-resource-type"></a>тип ресурса cloudPcGalleryImage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ресурс изображений галереи текущей организации, который можно использовать для обеспечения облачного компьютера.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки galleryImages](../api/virtualendpoint-list-deviceimages.md)|[коллекция cloudPcDeviceImage](../resources/cloudpcgalleryimage.md)|Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcgalleryimage.md)|
|[Get cloudPcGalleryImage](../api/cloudpcgalleryimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcgalleryimage.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcDeviceImage.](../resources/cloudpcgalleryimage.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Официальное имя отображения изображения галереи. Только для чтения.|
|endDate|Date|Дата, в которой это изображение больше не находится в долгосрочной поддержке. Облачный КОМПЬЮТЕР будет по-прежнему предоставлять кратковременную поддержку. Только для чтения.|
|expirationDate|Дата|Дата, когда изображение больше не доступно. Только для чтения.|
|id|Строка|Уникальный идентификатор для ресурса изображений галереи на облачном компьютере. Только для чтения.|
|предложение|Строка|Имя предложения изображения галереи. Это значение будет передано Azure для получения ресурса изображений. Только для чтения.|
|offerDisplayName|Строка|Официальное отображение предлагает имя изображения галереи. Например, Windows 10 Корпоративная оптимизация ОС. Только для чтения.|
|publisher|String|Имя издателя изображения галереи. Это значение будет передано Azure для получения ресурса изображений. Только для чтения.|
|recommendedSku|Строка|Рекомендуемый SKU облачного ПК для этого изображения галереи. Только для чтения.|
|sizeInGB|Int32|Размер этого изображения в гигабайтах. Только для чтения.|
|sku|Строка|Имя SKU изображения галереи. Это значение будет передано Azure для получения ресурса изображений. Только для чтения.|
|skuDisplayName|Строка|Официальное имя единицы сохраняющихся запасов (SKU) этого изображения галереи. Например, 2004 год. Только для чтения.|
|startDate|Date|Дата, когда изображение станет доступным. Только для чтения.|
|status|cloudPcGalleryImageStatus|Состояние изображения галереи на облачном компьютере. Возможные значения: `supported`, `supportedWithWarning`, `notSupported`, `unknownFutureValue`. Только для чтения.|

### <a name="cloudpcgalleryimagestatus-values"></a>значения cloudPcGalleryImageStatus

|Member|Описание|
|:---|:---|
|поддерживается|Изображение галереи активно и готово для использования для предварительной проготовки.|
|supportedWithWarning|Срок действия изображения галереи истек, но облачный компьютер будет поддерживаться в течение 6 месяцев, после чего он не будет поддерживаться и не может использоваться.|
|notSupported|Изображение галереи не поддерживается. |
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcGalleryImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName":"String",
  "offerDisplayName":"String",
  "skuDisplayName":"String",
  "publisher":"String",
  "offer":"String",
  "sku":"String",
  "recommendedSku":"String",
  "status":"String",
  "sizeInGB":"Int32",
  "startDate":"String (Date)",
  "endDate":"String (Date)",
  "expiredDate":"String (Date)"
}
```
