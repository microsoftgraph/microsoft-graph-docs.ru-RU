---
title: тип ресурса userExperienceAnalyticsBatteryHealthCapacityDetails
description: Объект емкости батареи для аналитики пользовательского интерфейса содержит количество устройств, разбитых на 3 категории, — устройства с емкостью > 80%, устройства с емкостью 50-80% и устройства с < 50%. Этот API предоставляет количество устройств в этих 3 категориях..
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f209ebf889bccaddf8f234a6858debf023ec6b3
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292020"
---
# <a name="userexperienceanalyticsbatteryhealthcapacitydetails-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthCapacityDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект емкости батареи для аналитики пользовательского интерфейса содержит количество устройств, разбитых на 3 категории, — устройства с емкостью > 80%, устройства с емкостью 50-80% и устройства с < 50%. Этот API предоставляет количество устройств в этих 3 категориях..

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get userExperienceAnalyticsBatteryHealthCapacityDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails-get.md)|[userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|Ознакомьтесь с свойствами и отношениями [объекта userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) .|
|[Обновление userExperienceAnalyticsBatteryHealthCapacityDetails](../api/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails-update.md)|[userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта емкости аккумулятора для аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств в клиенте. Допустимые значения 2147483648 2147483647|
|batteryCapacityGood|Int32|Количество устройств, максимальная емкость которых превышает 80%. Допустимые значения 2147483648 2147483647|
|batteryCapacityFair|Int32|Количество устройств, максимальная емкость которых превышает 50%, но меньше 80%. Допустимые значения 2147483648 2147483647|
|batteryCapacityPoor|Int32|Количество устройств, максимальная емкость которых составляет менее 50%. Допустимые значения 2147483648 2147483647|
|lastRefreshedDateTime|DateTimeOffset|Записано время даты этого экземпляра сведений о емкости.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "batteryCapacityGood": 1024,
  "batteryCapacityFair": 1024,
  "batteryCapacityPoor": 1024,
  "lastRefreshedDateTime": "String (timestamp)"
}
```




