---
title: vulnerableManagedDevice resource type
description: Эта сущность представляет устройство, связанное с задачей.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e6b498248d3143c6313ba97b839f7f6918a3af1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068650"
---
# <a name="vulnerablemanageddevice-resource-type"></a>vulnerableManagedDevice resource type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность представляет устройство, связанное с задачей.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список уязвимыхManagedDevices](../api/intune-partnerintegration-vulnerablemanageddevice-list.md)|[vulnerableManagedDevice collection](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Список свойств и связей уязвимых [объектовManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|
|[Get vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-get.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Чтение свойств и связей уязвимого [объектаManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|
|[Создание vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-create.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Создайте новый [объект vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|
|[Удаление vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-delete.md)|Нет|Удаляет [уязвимыйManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).|
|[Обновление vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-update.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Обновление свойств уязвимого [объектаManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности и ID устройства AAD.|
|managedDeviceId|Строка|ID управляемого устройства Intune.|
|displayName|Строка|Имя устройства.|
|lastSyncDateTime|DateTimeOffset|Последняя дата синхронизации.|

## <a name="relationships"></a>Отношения
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



