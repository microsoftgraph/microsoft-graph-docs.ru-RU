---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
ms.openlocfilehash: 756600ce2d48d77ec404bf3b8eb3ce123b142f3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076084"
---
# <a name="detectedapp-resource-type"></a>Тип ресурса detectedApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список detectedApps](../api/intune-devices-detectedapp-list.md)|Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)|Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Получение detectedApp](../api/intune-devices-detectedapp-get.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Создание объекта detectedApp](../api/intune-devices-detectedapp-create.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Удаление объекта detectedApp](../api/intune-devices-detectedapp-delete.md)|Нет|Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).|
|[Обновление detectedApp](../api/intune-devices-detectedapp-update.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для обнаруженного приложения. Он создается Intune автоматически при создании приложения. Только для чтения.|
|displayName|String|Имя обнаруженного приложения. Только для чтения|
|version|String|Версия обнаруженного приложения. Только для чтения|
|sizeInByte|Int64|Размер обнаруженного приложения в байтах. Только для чтения|
|deviceCount|Int32|Количество устройств, на которых было успешно установлено это приложение.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Устройства, на которых установлено обнаруженное приложение|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```





