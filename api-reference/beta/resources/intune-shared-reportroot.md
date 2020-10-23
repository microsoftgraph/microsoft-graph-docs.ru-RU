---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28d030eaf52f1656d4ba7da91c7cb3f6371958e3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726279"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-shared-reportroot-get.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-shared-reportroot-update.md)|Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|**Конфигурация устройств**|
|[Функция deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|[Функция deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|Метаданные для отчета о работе устройств|
|**Устранение неполадок**|
|[Функция Манажеддевицеенроллментабандонментдетаилс](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о прекращении регистрации|
|[Функция Манажеддевицеенроллментабандонментсуммари](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[report](../resources/intune-shared-report.md)|Метаданные для сводного отчета об отмене регистрации|
|[Функция Манажеддевицеенроллментфаилуредетаилс](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Пока не задокументировано.|
|[Функция Манажеддевицеенроллментфаилуретрендс](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Метаданные отчета о тенденциях сбоев регистрации|
|[Функция Манажеддевицеенроллменттопфаилурес](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Н/Д|

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





