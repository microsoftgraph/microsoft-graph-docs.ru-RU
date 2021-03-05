---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр отчетов журнала.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fe26bc7b5effb24fb0855da6d84b464f36de4927
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472036"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс, представляющий экземпляр отчетов журнала.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|**Конфигурация устройств**|
|[Функция deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о действиях устройств с конфигурацией устройств|
|[Функция deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|**Устранение неполадок**|
|[функция managedDeviceEnrollmentFailureDetails](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune-shared-report.md)|Еще не задокументировано.|
|[функция managedDeviceEnrollmentTopFailures](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/intune-shared-report.md)|Еще не задокументировано.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Пример

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```






