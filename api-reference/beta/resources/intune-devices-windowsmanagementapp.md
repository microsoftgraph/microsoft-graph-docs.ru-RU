---
title: Тип ресурса windowsManagementApp
description: Сущность приложения управления Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3db66a737e86ad66e66be8b9bde88e6024f8233
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983994"
---
# <a name="windowsmanagementapp-resource-type"></a>Тип ресурса windowsManagementApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Чтение свойств и связей объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .|
|[Обновление windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Обновление свойств объекта [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для приложения управления Windows|
|availableVersion|String|Доступная версия приложения управления Windows.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|healthSummary|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Сводка по работоспособности для приложения управления Windows.|
|healthStates|Коллекция [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md)|Список состояний работоспособности для установленного приложения управления Windows.|

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





