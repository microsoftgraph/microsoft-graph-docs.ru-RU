---
title: тип ресурса userExperienceAnalyticsWorkFromAnywhereModelPerformance
description: Аналитика пользовательских интерфейсов работает с любой производительности модели.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c6a21965c5f1f947b2f3d66dafcfb03cb777fc9
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292416"
---
# <a name="userexperienceanalyticsworkfromanywheremodelperformance-resource-type"></a>тип ресурса userExperienceAnalyticsWorkFromAnywhereModelPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательских интерфейсов работает с любой производительности модели.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsWorkFromAnywhereModelPerformances](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-list.md)|[коллекция userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|
|[Get userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-get.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|
|[Создание userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-create.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Создание нового [объекта userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|
|[Удаление userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md).|
|[Обновление userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-update.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности модели аналитики пользовательских интерфейсов.|
|model|String|Пользовательский интерфейс работает с любого типового имени устройств.|
|manufacturer|String|Пользовательский интерфейс работает с любого имени производителя устройств.|
|modelDeviceCount|Int32|Пользовательский опыт работы с устройств в любом месте считается для модели. Допустимые значения 2147483648 2147483647|
|workFromAnywhereScore|Double|Пользовательский опыт работы с любой общей оценкой для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|WindowsScore|Double|Пользовательский опыт работы из любого окна оценка для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudManagementScore|Double|Пользовательский опыт работы с любой оценкой облачного управления для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudIdentityScore|Double|Пользовательский опыт работы с облачной оценкой удостоверений в любом месте для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudProvisioningScore|Double|Пользовательский опыт работы с облачной оценкой для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние состояния аналитики пользовательских интерфейсов работает из любой модели. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance",
  "id": "String (identifier)",
  "model": "String",
  "manufacturer": "String",
  "modelDeviceCount": 1024,
  "workFromAnywhereScore": "4.2",
  "windowsScore": "4.2",
  "cloudManagementScore": "4.2",
  "cloudIdentityScore": "4.2",
  "cloudProvisioningScore": "4.2",
  "healthStatus": "String"
}
```




