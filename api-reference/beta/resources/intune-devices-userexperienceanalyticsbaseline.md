---
title: Тип ресурса Усерекспериенцеаналитиксбаселине
description: Базовый объект анализа пользовательского интерфейса содержит значения базовых показателей, на которые сравниваются показатели аналитики взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6063deec10d13c45565898f111d15ab6023b8838
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725409"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксбаселине

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый объект анализа пользовательского интерфейса содержит значения базовых показателей, на которые сравниваются показатели аналитики взаимодействия с пользователем.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксбаселинес](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|Коллекция [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Список свойств и связей объектов [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|
|[Получение Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|
|[Создание Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Создание нового объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|
|[Удаление Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md).|
|[Обновление Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Обновление свойств объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор базового идентификатора аналитики взаимодействия с пользователем.|
|displayName|Строка|Имя базового объекта аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель базового уровня для аналитики взаимодействия с пользователем.|
|isBuiltIn|Boolean|Указывает, является ли текущий базовый планом коммерческого медианы или настраиваемым базовым планом.|
|createdDateTime|DateTimeOffset|Дата создания настраиваемого базового плана.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|девицебутперформанцеметрикс|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Метрики производительности при загрузке устройств с помощью службы аналитики.|
|бестпрактицесметрикс|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели рекомендаций по анализу взаимодействия с пользователем.|
|ребутаналитиксметрикс|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Метрики аналитики взаимодействия с пользователем при перезагрузке.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "isBuiltIn": true,
  "createdDateTime": "String (timestamp)"
}
```





