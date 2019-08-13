---
title: Тип ресурса Усерекспериенцеаналитиксбаселине
description: Базовый объект анализа пользовательского интерфейса содержит значения базовых показателей, на которые сравниваются показатели аналитики взаимодействия с пользователем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce77b448d381547bfc77b6a27e1e9935f252be5e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371550"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксбаселине

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый объект анализа пользовательского интерфейса содержит значения базовых показателей, на которые сравниваются показатели аналитики взаимодействия с пользователем.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксбаселинес](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|Коллекция [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Список свойств и связей объектов [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|
|[Получение Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|
|[Создание Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Создание нового объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|
|[Удаление Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md).|
|[Обновление Усерекспериенцеаналитиксбаселине](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md)|Обновление свойств объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор базового идентификатора аналитики взаимодействия с пользователем.|
|displayName|Строка|Имя базового объекта аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель базового уровня для аналитики взаимодействия с пользователем.|
|овераллрегрессионсрешолд|Int32|Общее пороговое значение базовой регрессии базового интерфейса аналитики взаимодействия с пользователем.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|девицебутперформанцеметрикс|[усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md)|Метрики производительности при загрузке устройств с помощью службы аналитики.|
|бестпрактицесметрикс|[усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md)|Показатели рекомендаций по анализу взаимодействия с пользователем.|

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
  "overallRegressionThreshold": 1024
}
```



