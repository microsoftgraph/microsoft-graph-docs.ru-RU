---
title: Тип ресурса deviceManagement
description: Ресурс deviceManagement представляет идентификаторы устройств из коллекции клиента, которые были предварительно подготовлены в Intune, и профили регистрации, которые можно назначать идентификаторам устройств, поддерживающим конфигурацию до регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0102a098760e303267cc2e510e4e18a4a320126
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452876"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс deviceManagement представляет идентификаторы устройств из коллекции клиента, которые были предварительно подготовлены в Intune, и профили регистрации, которые можно назначать идентификаторам устройств, поддерживающим конфигурацию до регистрации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-enrollment-devicemanagement-get.md)|[deviceManagement](../resources/intune-enrollment-devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-enrollment-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-enrollment-devicemanagement-update.md)|[deviceManagement](../resources/intune-enrollment-devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune-enrollment-devicemanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|windowsAutopilotDeviceIdentities|[коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Идентификаторы Windows автопилота содержали коллекцию.|
|importedWindowsAutopilotDeviceIdentities|Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)|Коллекция импортированных устройств Windows AutoPilot.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



