---
title: Тип ресурса Клаудпкдевицеимаже
description: Представляет ресурс изображения на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 600fceffadb03247c646b2728e445c0c07cae9aa
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378645"
---
# <a name="cloudpcdeviceimage-resource-type"></a>Тип ресурса Клаудпкдевицеимаже

Пространство имен: microsoft.graph

Представляет ресурс изображения на облачном компьютере.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Девицеимажес](../api/virtualendpoint-list-deviceimages.md)|Коллекция [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)|Перечисление свойств и связей объектов [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .|
|[Получение Клаудпкдевицеимаже](../api/cloudpcdeviceimage-get.md)|[клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)|Чтение свойств и связей объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .|
|[Создание Клаудпкдевицеимаже](../api/virtualendpoint-post-deviceimages.md)|[клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)|Создание нового объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .|
|[Удаление Клаудпкдевицеимаже](../api/cloudpcdeviceimage-delete.md)|Нет|Удаление объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .|
|[жетсаурцеимажес](../api/cloudpcdeviceimage-getsourceimages.md)|Коллекция [клаудпксаурцедевицеимаже](../resources/cloudpcsourcedeviceimage.md)|Получение объектов [клаудпксаурцедевицеимаже](../resources/cloudpcsourcedeviceimage.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор ресурса изображения на облачном компьютере. Только для чтения.|
|саурцеимажересаурцеид|Строка|Идентификатор исходного ресурса изображения в Azure. Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.компуте/имажес/{имаженаме}".|
|displayName|Строка|Отображаемое имя изображения.|
|version|String|Версия изображения. Например: 0.0.1, 1.5.13.|
|осбуилднумбер|Строка|Версия сборки ОС образа. Пример: 1909.|
|operatingSystem|String|Операционная система изображения. Пример: Windows 10 Корпоративная.|
|lastModifiedDateTime|DateTimeOffset|Данные и время последнего изменения изображения. Время отображается в формате ISO 8601 и времени в формате UTC. Например, полночь UTC 1 января 2014 отображается как "2014 – 01 – 01T00:00:00Z".|
|status|клаудпкдевицеимажестатус|Состояние изображения на облачном ПК. Возможные состояния: Ожидание отправки, сбой отправки или готовность к использованию. Возможные значения: `pending`, `ready`, `failed`.|
|статусдетаилс|клаудпкдевицеимажестатусдетаилс|Сведения о состоянии изображения, указывающие на неудачную отправку, если это возможно. Возможные значения: `internalServerError`, `sourceImageNotFound`.|

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
