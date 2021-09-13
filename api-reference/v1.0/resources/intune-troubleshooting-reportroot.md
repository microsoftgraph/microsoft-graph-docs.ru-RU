---
title: Тип ресурса reportRoot
description: Ресурс, представляючий экземпляр отчетов о сбоях регистрации.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0545c2f2b0fbabc03fbc2b628a9d1752fc3f0748
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021514"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс, представляючий экземпляр отчетов о сбоях регистрации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-troubleshooting-reportroot-get.md)|[reportRoot](../resources/intune-troubleshooting-reportroot.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-troubleshooting-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-troubleshooting-reportroot-update.md)|[reportRoot](../resources/intune-troubleshooting-reportroot.md)|Обновление свойств объекта [reportRoot](../resources/intune-troubleshooting-reportroot.md).|
|[функция managedDeviceEnrollmentFailureDetails](../api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune-troubleshooting-report.md)|Пока не задокументировано.|
|[функция managedDeviceEnrollmentFailureDetails](../api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune-troubleshooting-report.md)|Пока не задокументировано.|
|[функция managedDeviceEnrollmentTopFailures](../api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/intune-troubleshooting-report.md)|Пока не задокументировано.|
|[функция managedDeviceEnrollmentTopFailures](../api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/intune-troubleshooting-report.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этого объекта.|

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




