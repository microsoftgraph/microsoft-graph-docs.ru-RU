---
title: тип ресурса macOSSoftwareUpdateStateSummary
description: Сводка состояния состояния программного обеспечения MacOS для устройства и пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc9ea010e664ab2cd2094dfca69152455cd61d9d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784844"
---
# <a name="macossoftwareupdatestatesummary-resource-type"></a>тип ресурса macOSSoftwareUpdateStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка состояния состояния программного обеспечения MacOS для устройства и пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSSoftwareUpdateStateSummaries](../api/intune-deviceconfig-macossoftwareupdatestatesummary-list.md)|[коллекция macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Список свойств и связей объектов [macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|
|[Get macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Чтение свойств и связей объекта [macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|
|[Создание macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Создайте новый [объект macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|
|[Удаление macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|Нет|Удаляет [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).|
|[Обновление macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Обновление свойств объекта [macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|Строка|Понятное для человека имя обновления программного обеспечения|
|productKey|String|Ключ продукта обновления программного обеспечения.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Категория обновления программного обеспечения. Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.|
|updateVersion|Строка|Версия обновления программного обеспечения|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Состояние обновления программного обеспечения. Возможные значения: `success` `downloading` , , , , , `downloaded` , `installing` , `idle` `available` `scheduled` `downloadFailed` `downloadInsufficientSpace` , `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` , .|
|lastUpdatedDateTime|DateTimeOffset|Последний раз, когда отчет для этого устройства и ключ продукта был обновлен.|

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



