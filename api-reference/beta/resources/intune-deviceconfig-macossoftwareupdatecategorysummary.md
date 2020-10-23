---
title: Тип ресурса Макоссофтвареупдатекатегорисуммари
description: Сводный отчет по категории обновлений программного обеспечения MacOS для устройства и пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bce8f433ef965a0ef90acc72691e31e707d9293
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735262"
---
# <a name="macossoftwareupdatecategorysummary-resource-type"></a>Тип ресурса Макоссофтвареупдатекатегорисуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводный отчет по категории обновлений программного обеспечения MacOS для устройства и пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макоссофтвареупдатекатегорисуммариес](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-list.md)|Коллекция [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Список свойств и связей объектов [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .|
|[Получение Макоссофтвареупдатекатегорисуммари](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-get.md)|[макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Чтение свойств и связей объекта [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .|
|[Создание Макоссофтвареупдатекатегорисуммари](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-create.md)|[макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Создание нового объекта [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .|
|[Удаление Макоссофтвареупдатекатегорисуммари](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-delete.md)|Нет|Удаляет объект [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).|
|[Обновление Макоссофтвареупдатекатегорисуммари](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-update.md)|[макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Обновление свойств объекта [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Имя отчета|
|deviceId|String|ИДЕНТИФИКАТОР устройства.|
|userId|String|Идентификатор пользователя.|
|упдатекатегори|[макоссофтвареупдатекатегори](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Тип обновления программного обеспечения. Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.|
|сукцессфулупдатекаунт|Int32|Количество успешных обновлений на устройстве|
|фаиледупдатекаунт|Int32|Количество неудачных обновлений на устройстве|
|тоталупдатекаунт|Int32|Общее количество обновлений на устройстве|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления отчета для этого устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|упдатестатесуммариес|Коллекция [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Сводка состояний обновлений.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateCategorySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "String (identifier)",
  "displayName": "String",
  "deviceId": "String",
  "userId": "String",
  "updateCategory": "String",
  "successfulUpdateCount": 1024,
  "failedUpdateCount": 1024,
  "totalUpdateCount": 1024,
  "lastUpdatedDateTime": "String (timestamp)"
}
```





