---
title: тип ресурса userExperienceAnalyticsImpactingProcess
description: Аналитика пользовательского интерфейса оказывает влияние на объект процесса.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d61d647db49c61960afdd15d9401138f465d662a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125696"
---
# <a name="userexperienceanalyticsimpactingprocess-resource-type"></a>тип ресурса userExperienceAnalyticsImpactingProcess

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Аналитика пользовательского интерфейса оказывает влияние на объект процесса.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsImpactingProcesses](../api/intune-devices-userexperienceanalyticsimpactingprocess-list.md)|[коллекция userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Список свойств и связей [объектов userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|
|[Get userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-get.md)|[userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Чтение свойств и связей [объекта userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|
|[Создание userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-create.md)|[userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Создание нового [объекта userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|
|[Удаление userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).|
|[Обновление userExperienceAnalyticsImpactingProcess](../api/intune-devices-userexperienceanalyticsimpactingprocess-update.md)|[userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|Обновление свойств объекта [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта аналитики пользовательского интерфейса, который оказывает влияние на процесс.|
|deviceId|String|Уникальный идентификатор влияемого устройства.|
|category|String|Категория воздействия процесса.|
|processName|String|Имя процесса.|
|description|String|Описание процесса.|
|publisher|String|Издатель процесса.|
|impactValue|Двойное с плавающей точкой|Значение влияния процесса. Допустимые значения от 0 до 1.79769313486232E+308|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsImpactingProcess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "String (identifier)",
  "deviceId": "String",
  "category": "String",
  "processName": "String",
  "description": "String",
  "publisher": "String",
  "impactValue": "4.2"
}
```



