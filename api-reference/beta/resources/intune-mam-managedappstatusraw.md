---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 557992bcec9ddc090d00189fa2044fc6e37e3a67
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43371734"
---
# <a name="managedappstatusraw-resource-type"></a>Тип ресурса managedAppStatusRaw

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.


Наследуется от [managedAppStatus](../resources/intune-mam-managedappstatus.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedAppStatusRaws](../api/intune-mam-managedappstatusraw-list.md)|Коллекция [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|
|[Получение managedAppStatusRaw](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Понятное имя отчета о состоянии. Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|content|[Json](../resources/intune-mam-json.md)|Содержимое отчета о состоянии.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



