---
title: Тип ресурса Макоссофтвареупдатестатесуммари
description: Сводка по состоянию обновления программного обеспечения MacOS для устройства и пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6cadcfa190f2f2c665a9671c9c9f17f94d646d04
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705133"
---
# <a name="macossoftwareupdatestatesummary-resource-type"></a>Тип ресурса Макоссофтвареупдатестатесуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по состоянию обновления программного обеспечения MacOS для устройства и пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макоссофтвареупдатестатесуммариес](../api/intune-deviceconfig-macossoftwareupdatestatesummary-list.md)|Коллекция [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Список свойств и связей объектов [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Получение Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Чтение свойств и связей объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Создание Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Создание нового объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Удаление Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|Нет|Удаляет объект [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).|
|[Обновление Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Обновление свойств объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Понятное имя обновления программного обеспечения|
|productKey|String|Ключ продукта обновления программного обеспечения.|
|упдатекатегори|[макоссофтвареупдатекатегори](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Категория обновлений программного обеспечения. Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.|
|упдатеверсион|Строка|Версия обновления программного обеспечения|
|state|[макоссофтвареупдатестате](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Состояние обновления программного обеспечения. Возможные значения: `success` , `downloading` ,,,,, `downloaded` `installing` `idle` `available` `scheduled` ,,, `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` , `downloadInsufficientNetwork` , `installInsufficientSpace` , `installInsufficientPower` , `installFailed` , `commandFailed` .|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления отчета для этого устройства и ключа продукта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "productKey": "String",
  "updateCategory": "String",
  "updateVersion": "String",
  "state": "String",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





