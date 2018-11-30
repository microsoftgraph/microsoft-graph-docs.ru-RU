---
title: Тип ресурса managedAppStatusRaw
description: Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.
ms.openlocfilehash: ba2f398e54e27cb079dd575530d46a7bf287722d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075117"
---
# <a name="managedappstatusraw-resource-type"></a>Тип ресурса managedAppStatusRaw

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|displayName|String|Понятное имя отчета о состоянии. Наследуется от объекта [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
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





