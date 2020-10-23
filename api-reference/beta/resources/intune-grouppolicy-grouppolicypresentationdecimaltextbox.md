---
title: Тип ресурса ГраупполиципресентатиондеЦималтекстбокс
description: Представляет элемент ADMX ДеЦималтекстбокс и десятичный элемент ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 197d5a2d068e685d8d4929d9e9ebe0ed8af874af
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684689"
---
# <a name="grouppolicypresentationdecimaltextbox-resource-type"></a>Тип ресурса ГраупполиципресентатиондеЦималтекстбокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент ADMX ДеЦималтекстбокс и десятичный элемент ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ГраупполиципресентатиондеЦималтекстбоксес](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-list.md)|Коллекция [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Список свойств и связей объектов [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .|
|[Получение ГраупполиципресентатиондеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-get.md)|[граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Чтение свойств и связей объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .|
|[Создание ГраупполиципресентатиондеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-create.md)|[граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Создание нового объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .|
|[Удаление ГраупполиципресентатиондеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-delete.md)|Нет|Удаляет объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).|
|[Обновление ГраупполиципресентатиондеЦималтекстбокс](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-update.md)|[граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|Обновление свойств объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|Строка|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|Int64|Целое число без знака, задающее начальное значение для десятичного текстового поля. Значение по умолчанию равно 1.|
|повернуть|Логический|Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента. Значение по умолчанию: true.|
|спинстеп|Int64|Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик". Значение по умолчанию равно 1.|
|Обязательный|Логический|Требование ввести значение в поле параметр. Значение по умолчанию  false.|
|minValue|Int64|Целое число без знака, задающее минимальное допустимое значение. Значение по умолчанию равно 0.|
|maxValue|Int64|Целое число без знака, задающее максимальное допустимое значение. Значение по умолчанию — 9999.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
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





