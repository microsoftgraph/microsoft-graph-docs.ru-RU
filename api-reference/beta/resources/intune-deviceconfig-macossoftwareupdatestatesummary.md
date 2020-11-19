---
title: Тип ресурса Макоссофтвареупдатестатесуммари
description: Сводка по состоянию обновления программного обеспечения MacOS для устройства и пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb7cebab56f9866753794259b70a0bdd8cc1e414
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279817"
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
|[Получение Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Чтение свойств и связей объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Создание Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Создание нового объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Удаление Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|Нет|Удаляет объект [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).|
|[Обновление Макоссофтвареупдатестатесуммари](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Обновление свойств объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Понятное имя обновления программного обеспечения|
|productKey|String|Ключ продукта обновления программного обеспечения.|
|упдатекатегори|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Категория обновлений программного обеспечения. Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.|
|упдатеверсион|String|Версия обновления программного обеспечения|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Состояние обновления программного обеспечения. Возможные значения: `success` , `downloading` ,,,,, `downloaded` `installing` `idle` `available` `scheduled` ,,, `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` , `downloadInsufficientNetwork` , `installInsufficientSpace` , `installInsufficientPower` , `installFailed` , `commandFailed` .|
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




