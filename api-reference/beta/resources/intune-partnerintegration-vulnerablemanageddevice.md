---
title: Тип ресурса Вулнераблеманажеддевице
description: Эта сущность представляет устройство, связанное с задачей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc6bd83d3ffbf49039f4e2fef9722f49d853f377
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709868"
---
# <a name="vulnerablemanageddevice-resource-type"></a>Тип ресурса Вулнераблеманажеддевице

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность представляет устройство, связанное с задачей.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Вулнераблеманажеддевицес](../api/intune-partnerintegration-vulnerablemanageddevice-list.md)|Коллекция [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Список свойств и связей объектов [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|
|[Получение Вулнераблеманажеддевице](../api/intune-partnerintegration-vulnerablemanageddevice-get.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Чтение свойств и связей объекта [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|
|[Создание Вулнераблеманажеддевице](../api/intune-partnerintegration-vulnerablemanageddevice-create.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Создание нового объекта [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|
|[Удаление Вулнераблеманажеддевице](../api/intune-partnerintegration-vulnerablemanageddevice-delete.md)|Нет|Удаляет объект [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md).|
|[Обновление Вулнераблеманажеддевице](../api/intune-partnerintegration-vulnerablemanageddevice-update.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Обновление свойств объекта [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ сущности и идентификатор устройства AAD.|
|манажеддевицеид|Строка|Идентификатор управляемого устройства Intune.|
|displayName|Строка|Имя устройства.|
|lastSyncDateTime|DateTimeOffset|Дата последней синхронизации.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vulnerableManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "displayName": "String",
  "lastSyncDateTime": "String (timestamp)"
}
```





