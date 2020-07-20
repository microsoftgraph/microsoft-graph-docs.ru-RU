---
title: Тип ресурса Девицекомплианцескрипт
description: Intune предоставит клиенту возможность выполнять сценарии соответствия PowerShell (обнаружение) на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aba8998ff1615741e481924a6602dc10f0171371
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789568"
---
# <a name="devicecompliancescript-resource-type"></a>Тип ресурса Девицекомплианцескрипт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность выполнять сценарии соответствия PowerShell (обнаружение) на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицекомплианцескриптс](../api/intune-devices-devicecompliancescript-list.md)|Коллекция [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md)|Список свойств и связей объектов [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .|
|[Получение Девицекомплианцескрипт](../api/intune-devices-devicecompliancescript-get.md)|[девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md)|Чтение свойств и связей объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .|
|[Создание Девицекомплианцескрипт](../api/intune-devices-devicecompliancescript-create.md)|[девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md)|Создание нового объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .|
|[Удаление Девицекомплианцескрипт](../api/intune-devices-devicecompliancescript-delete.md)|Нет|Удаляет объект [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md).|
|[Обновление Девицекомплианцескрипт](../api/intune-devices-devicecompliancescript-update.md)|[девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md)|Обновление свойств объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .|
|[Действие assign](../api/intune-devices-devicecompliancescript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для сценария соответствия требованиям устройства|
|publisher|String|Имя издателя сценариев соответствия требованиям устройства|
|version|String|Версия сценария соответствия требованиям устройства|
|displayName|Строка|Имя сценария соответствия требованиям устройства|
|description|String|Описание сценария соответствия требованиям устройства|
|детектионскриптконтент|Binary|Весь контент скрипта обнаружения PowerShell|
|createdDateTime|DateTimeOffset|Метка времени создания сценария соответствия устройства требованиям. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Метка времени изменения сценария соответствия требованиям устройства. Это свойство доступно только для чтения.|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Boolean|Указывает, нужно ли проверять подпись скрипта|
|runAs32Bit|Boolean|Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для сценария соответствия требованиям устройств|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md)|Список назначений групп для сценария соответствия требованиям к устройствам|
|Свойства навигации runsummary|[девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Сводка по выполнению высокого уровня для сценария соответствия требованиям устройства.|
|deviceRunStates|Коллекция [девицекомплианцескриптдевицестате](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Список состояний запуска для сценария соответствия требованиям устройств для всех устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



