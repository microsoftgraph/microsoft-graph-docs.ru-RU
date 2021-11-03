---
title: тип ресурса userExperienceAnalyticsBatteryHealthRuntimeDetails
description: 'Объект для аналитики состояния заряда батареи для пользователей содержит количество устройств, разбитых на 3 категории : устройства с > 5 часов, устройства с временем работы 3-5 часов и устройства с < 3 часа. Этот API предоставляет количество устройств в этих 3 категориях.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: abad7a43373f572b8b6880ceb36d9463b2cdb8e7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697427"
---
# <a name="userexperienceanalyticsbatteryhealthruntimedetails-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthRuntimeDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект для аналитики состояния заряда батареи для пользователей содержит количество устройств, разбитых на 3 категории : устройства с > 5 часов, устройства с временем работы 3-5 часов и устройства с < 3 часа. Этот API предоставляет количество устройств в этих 3 категориях.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get userExperienceAnalyticsBatteryHealthRuntimeDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails-get.md)|[userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|Чтение свойств и связей [объекта userExperienceAnalyticsBatteryHealthRuntimeDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|
|[Обновление userExperienceAnalyticsBatteryHealthRuntimeDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails-update.md)|[userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthRuntimeDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта для аналитики пользовательского интерфейса для запуска заряда батареи.|
|activeDevices|Int32|Количество активных устройств в клиенте. Допустимые значения 2147483648 2147483647|
|batteryRuntimeGood|Int32|Количество устройств, время активного запуска которых превышает 5 часов. Допустимые значения 2147483648 2147483647|
|batteryRuntimeFair|Int32|Количество устройств, время активного запуска которых превышает 3 часа, но меньше 5 часов. Допустимые значения 2147483648 2147483647|
|batteryRuntimePoor|Int32|Количество устройств, время активного запуска которых меньше 3 часов. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "batteryRuntimeGood": 1024,
  "batteryRuntimeFair": 1024,
  "batteryRuntimePoor": 1024
}
```



