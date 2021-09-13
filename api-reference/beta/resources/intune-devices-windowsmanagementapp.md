---
title: тип ресурса windowsManagementApp
description: Windows управления приложением.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86ee3906463d6d76fda1c961c04dd20fd3d790fa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091288"
---
# <a name="windowsmanagementapp-resource-type"></a>тип ресурса windowsManagementApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows управления приложением.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Чтение свойств и связей [объекта WindowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)|
|[Обновление WindowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Обновление свойств объекта [WindowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)|
|[действие setAsManagedInstaller](../api/intune-devices-windowsmanagementapp-setasmanagedinstaller.md)|Нет|Настройка состояния управляемого установщика для клиента вызываемого|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для приложения Windows управления|
|availableVersion|String|Windows доступной версии приложения для управления.|
|managedInstaller|[managedInstallerStatus](../resources/intune-devices-managedinstallerstatus.md)|Состояние управляемого установщика. Возможные значения: `disabled`, `enabled`.|
|managedInstallerConfiguredDateTime|String|Настроено время даты управляемого установщика|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|healthStates|[коллекция windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Список состояния здоровья для установленного приложения Windows управления.|

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
  "availableVersion": "String",
  "managedInstaller": "String",
  "managedInstallerConfiguredDateTime": "String"
}
```



