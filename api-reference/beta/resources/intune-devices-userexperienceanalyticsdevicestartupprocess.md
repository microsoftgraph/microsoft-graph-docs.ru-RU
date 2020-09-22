---
title: Тип ресурса Усерекспериенцеаналитиксдевицестартуппроцесс
description: Сведения о процессе запуска устройства Analytics User Experience.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9321c6b133d8017eef442944307de52f9f17ed78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080917"
---
# <a name="userexperienceanalyticsdevicestartupprocess-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксдевицестартуппроцесс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о процессе запуска устройства Analytics User Experience.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксдевицестартуппроцессес](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-list.md)|Коллекция [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|
|[Получение Усерекспериенцеаналитиксдевицестартуппроцесс](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-get.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|
|[Создание Усерекспериенцеаналитиксдевицестартуппроцесс](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-create.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|
|[Удаление Усерекспериенцеаналитиксдевицестартуппроцесс](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).|
|[Обновление Усерекспериенцеаналитиксдевицестартуппроцесс](../api/intune-devices-userexperienceanalyticsdevicestartupprocess-update.md)|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)|Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.|
|манажеддевицеид|Строка|Идентификатор устройства службы аналитики взаимодействия с пользователем.|
|процесснаме|Строка|Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.|
|productName|String|Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).|
|publisher|String|Издатель процесса запуска устройства Analytics User Experience.|
|стартупимпактинмс|Int32|Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupProcess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": 1024
}
```






