---
title: тип ресурса deviceManagementScriptRunSummary
description: Содержит свойства для сводки запуска скрипта управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a409bff5addf078e14352217b2bb9cdbeab6f74b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125955"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>тип ресурса deviceManagementScriptRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки запуска скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Чтение свойств и связей [объекта deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)|
|[Обновление deviceManagementScriptRunSummary](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Обновление свойств объекта [deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша скрипта управления устройствами запустит объект сводки. Это свойство доступно только для чтения.|
|successDeviceCount|Int32|Количество устройств успешности.|
|errorDeviceCount|Int32|Количество устройств ошибки.|
|successUserCount|Int32|Количество пользователей успешности.|
|errorUserCount|Int32|Количество пользователей ошибки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



