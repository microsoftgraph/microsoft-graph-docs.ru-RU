---
title: тип ресурса userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
description: Объект подготовки оборудования для аналитики пользовательских интерфейсов содержит сведения об уровне учетных записей об блокаторах оборудования для обновления Windows.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9716cee7e1ba03253b040c52d49e0df404b9c48
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046871"
---
# <a name="userexperienceanalyticsworkfromanywherehardwarereadinessmetric-resource-type"></a>тип ресурса userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект подготовки оборудования для аналитики пользовательских интерфейсов содержит сведения об уровне учетных записей об блокаторах оборудования для обновления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../api/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric-get.md)|[userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|Чтение свойств и связей объекта [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|
|[Обновление userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../api/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric-update.md)|[userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта метрики готовности оборудования для аналитики пользовательского интерфейса.|
|totalDeviceCount|Int32|Общее количество устройств в организации. Допустимые значения 2147483648 2147483647|
|upgradeEligibleDeviceCount|Int32|Количество устройств в организации, имеющих право на обновление Windows. Допустимые значения 2147483648 2147483647|
|ramCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка оборудования оперативной памяти не удалась. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|storageCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка оборудования хранения не удалась. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processorCoreCountCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка подсчета ядра процессорного оборудования не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processorSpeedCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка скорости работы процессорного оборудования не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|tpmCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка аппаратного модуля доверенных платформ (TPM) не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|secureBootCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых не удалось проверить безопасное оборудование загрузки. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processorFamilyCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых семейная проверка оборудования обработчика не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|processor64BitCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка архитектуры процессорного оборудования 64-битной архитектуры не удалось. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|osCheckFailedPercentage|Двойное с плавающей точкой|Процент устройств, для которых проверка ОС не удалась. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "id": "String (identifier)",
  "totalDeviceCount": 1024,
  "upgradeEligibleDeviceCount": 1024,
  "ramCheckFailedPercentage": "4.2",
  "storageCheckFailedPercentage": "4.2",
  "processorCoreCountCheckFailedPercentage": "4.2",
  "processorSpeedCheckFailedPercentage": "4.2",
  "tpmCheckFailedPercentage": "4.2",
  "secureBootCheckFailedPercentage": "4.2",
  "processorFamilyCheckFailedPercentage": "4.2",
  "processor64BitCheckFailedPercentage": "4.2",
  "osCheckFailedPercentage": "4.2"
}
```



