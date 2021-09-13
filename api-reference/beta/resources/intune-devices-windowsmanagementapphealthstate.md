---
title: тип ресурса windowsManagementAppHealthState
description: Windows объекта состояния состояния здоровья приложения управления.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 885827482bcf24bfe6b90c2feb564190e004975a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040038"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a>тип ресурса windowsManagementAppHealthState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows объекта состояния состояния здоровья приложения управления.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsManagementAppHealthStates](../api/intune-devices-windowsmanagementapphealthstate-list.md)|[коллекция windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Список свойств и связей объектов [WindowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|
|[Get windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Чтение свойств и связей [объекта WindowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|
|[Создание windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Создание нового [объекта WindowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|
|[Удаление windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|Нет|Удаляет [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).|
|[Обновление windowsManagementAppHealthState](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)|Обновление свойств объекта [windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор состояния Windows приложения управления. Это свойство доступно только для чтения.|
|healthState|[healthState](../resources/intune-devices-healthstate.md)|Windows состояния здоровья приложения управления. Возможные значения: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|String|Windows установленной версии приложения управления.|
|lastCheckInDateTime|DateTimeOffset|Windows последнего времени регистрации приложения управления.|
|deviceName|String|Имя устройства, на котором Windows установлено приложение управления.|
|deviceOSVersion|String|Windows 10 ВЕРСИЯ ОС устройства, на котором Windows установлено приложение управления.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```



