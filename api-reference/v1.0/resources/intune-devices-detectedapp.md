---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6e1d5f6ec6bab9b9506cf6ddcab625ff3d04b74
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758759"
---
# <a name="detectedapp-resource-type"></a>Тип ресурса detectedApp

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




