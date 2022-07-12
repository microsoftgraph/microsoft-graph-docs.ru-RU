---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр отчетов журнала.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efaf3832d6fd6a77f4a7f92dd208f8ffb02988cc
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735385"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс, представляющий экземпляр отчетов журнала.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-deviceconfig-reportroot-get.md)|[reportRoot](../resources/intune-deviceconfig-reportroot.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-deviceconfig-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-deviceconfig-reportroot-update.md)|[reportRoot](../resources/intune-deviceconfig-reportroot.md)|Обновление свойств объекта [reportRoot](../resources/intune-deviceconfig-reportroot.md).|
|[Функция deviceConfigurationUserActivity](../api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity.md)|[report](../resources/intune-deviceconfig-report.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|[Функция deviceConfigurationDeviceActivity](../api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity.md)|[report](../resources/intune-deviceconfig-report.md)|Метаданные для отчета о действиях устройств с конфигурацией устройств|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```





