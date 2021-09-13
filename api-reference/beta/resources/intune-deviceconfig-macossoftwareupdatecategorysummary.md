---
title: тип ресурса macOSSoftwareUpdateCategorySummary
description: Сводный отчет об обновлении программного обеспечения MacOS для устройства и пользователя
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f8d084eccf6e253c258f7ddd14c1c09feaa1ad2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095565"
---
# <a name="macossoftwareupdatecategorysummary-resource-type"></a>тип ресурса macOSSoftwareUpdateCategorySummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводный отчет об обновлении программного обеспечения MacOS для устройства и пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список macOSSoftwareUpdateCategorySummaries](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-list.md)|[коллекция macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Список свойств и связей объектов [macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|
|[Get macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-get.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Чтение свойств и связей объекта [macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|
|[Создание macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-create.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Создайте новый [объект macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|
|[Удаление macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-delete.md)|Нет|Удаляет [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).|
|[Обновление macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-update.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Обновление свойств объекта [macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя отчета|
|deviceId|String|ID устройства.|
|userId|String|Идентификатор пользователя.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Тип обновления программного обеспечения. Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.|
|successfulUpdateCount|Int32|Количество успешных обновлений на устройстве|
|failedUpdateCount|Int32|Количество сбойных обновлений на устройстве|
|totalUpdateCount|Int32|Количество обновлений на устройстве|
|lastUpdatedDateTime|DateTimeOffset|Последняя дата обновления отчета для этого устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|updateStateSummaries|[коллекция macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Сводка состояния обновления.|

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



