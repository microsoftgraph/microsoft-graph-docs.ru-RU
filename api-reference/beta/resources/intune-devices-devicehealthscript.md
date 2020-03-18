---
title: Тип ресурса Девицехеалсскрипт
description: Intune предоставит клиенту возможность выполнять сценарии работоспособности PowerShell (исправление и обнаружение) на зарегистрированных устройствах, подключенных к Windows 10 Azure Active Directory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80e1539cf941d2d1cfa04fefcb442493f984347c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784967"
---
# <a name="devicehealthscript-resource-type"></a>Тип ресурса Девицехеалсскрипт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность выполнять сценарии работоспособности PowerShell (исправление и обнаружение) на зарегистрированных устройствах, подключенных к Windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицехеалсскриптс](../api/intune-devices-devicehealthscript-list.md)|Коллекция [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md)|Список свойств и связей объектов [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Получение Девицехеалсскрипт](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Чтение свойств и связей объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Создание Девицехеалсскрипт](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Создание нового объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Удаление Девицехеалсскрипт](../api/intune-devices-devicehealthscript-delete.md)|Нет|Удаляет объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).|
|[Обновление Девицехеалсскрипт](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Действие assign](../api/intune-devices-devicehealthscript-assign.md)|Нет|Н/Д|
|[действие Упдатеглобалскрипт](../api/intune-devices-devicehealthscript-updateglobalscript.md)|String|Обновление сценария работоспособности собственного устройства|
|[действие Жетглобалскрипсигхеставаилаблеверсион](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|String|Обновление сценария работоспособности собственного устройства|
|[действие Енаблеглобалскриптс](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|Нет|Н/Д|
|[Функция Ареглобалскриптсаваилабле](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|Пока не задокументировано.|
|[Функция Жетремедиатионсуммари](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[девицехеалсскриптремедиатионсуммари](../resources/intune-devices-devicehealthscriptremediationsummary.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сценария работоспособности устройства|
|publisher|String|Имя издателя сценария работоспособности устройства|
|version|String|Версия сценария работоспособности устройства|
|displayName|Строка|Имя сценария работоспособности устройства|
|description|String|Описание сценария работоспособности устройства|
|детектионскриптконтент|Binary|Весь контент скрипта обнаружения PowerShell|
|ремедиатионскриптконтент|Binary|Все содержимое скрипта PowerShell об исправлении|
|createdDateTime|DateTimeOffset|Метка времени создания сценария работоспособности устройства. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Метка времени изменения сценария работоспособности устройства. Это свойство доступно только для чтения.|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Логический|Указывает, нужно ли проверять подпись скрипта|
|runAs32Bit|Логический|Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для сценария работоспособности устройства|
|исглобалскрипт|Логический|Определяет, является ли этот сценарий фирменным (Майкрософт). Специальные сценарии доступны только для чтения|
|хигхеставаилаблеверсион|String|Самая высокая доступная версия для собственного сценария Майкрософт|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)|Список назначений групп для сценария работоспособности устройства|
|Свойства навигации runsummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Сводка по выполнению высокого уровня для сценария работоспособности устройства.|
|deviceRunStates|Коллекция [девицехеалсскриптдевицестате](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список состояний запуска для сценария работоспособности устройства на всех устройствах|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String"
}
```



