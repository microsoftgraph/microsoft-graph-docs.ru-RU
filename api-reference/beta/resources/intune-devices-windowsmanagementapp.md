---
title: Тип ресурса windowsManagementApp
description: Сущность приложения управления Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a3b311863422e25b7b1f2d0dda4780f152ba2c74
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393013"
---
# <a name="windowsmanagementapp-resource-type"></a>Тип ресурса windowsManagementApp

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Чтение свойства и связи объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .|
|[Обновление windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Обновление свойства объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для приложения управления Windows|
|availableVersion|String|Управление приложения доступные версии Windows.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|healthSummary|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Работоспособности для приложения управления Windows.|
|healthStates|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) коллекции|Список состояния работоспособности для установленного приложения управления Windows.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```




