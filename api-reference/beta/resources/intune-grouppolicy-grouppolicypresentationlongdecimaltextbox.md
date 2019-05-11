---
title: Тип ресурса ГраупполиципресентатионлонгдеЦималтекстбокс
description: Представляет элемент ADMX ЛонгдеЦималтекстбокс и элемент ЛонгдеЦимал ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71e3f9cfe101c1c408bfdebdf7b2d0606f0a2231
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941053"
---
# <a name="grouppolicypresentationlongdecimaltextbox-resource-type"></a>Тип ресурса ГраупполиципресентатионлонгдеЦималтекстбокс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент ADMX ЛонгдеЦималтекстбокс и элемент ЛонгдеЦимал ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ГраупполиципресентатионлонгдеЦималтекстбоксес](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-list.md)|Коллекция [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Список свойств и связей объектов [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .|
|[Получение ГраупполиципресентатионлонгдеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-get.md)|[ГраупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Чтение свойств и связей объекта [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .|
|[Создание ГраупполиципресентатионлонгдеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-create.md)|[ГраупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Создание нового объекта [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .|
|[Удаление ГраупполиципресентатионлонгдеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).|
|[Обновление ГраупполиципресентатионлонгдеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-update.md)|[ГраупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Обновление свойств объекта [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|Строка|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|Int64|Целое число без знака, задающее начальное значение для десятичного текстового поля. Значение по умолчанию равно 1.|
|повернуть|Логический|Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента. Значение по умолчанию: true.|
|Спинстеп|Int64|Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик". Значение по умолчанию равно 1.|
|Обязательный|Логический|Требование ввести значение в поле параметр. Значение по умолчанию  false.|
|minValue|Int64|Длинное целое число без знака, задающее минимальное допустимое значение. Значение по умолчанию равно 0.|
|maxValue|Int64|Длинное целое число без знака, задающее максимальное допустимое значение. Значение по умолчанию — 9999.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationLongDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": 1024,
  "spin": true,
  "spinStep": 1024,
  "required": true,
  "minValue": 1024,
  "maxValue": 1024
}
```




