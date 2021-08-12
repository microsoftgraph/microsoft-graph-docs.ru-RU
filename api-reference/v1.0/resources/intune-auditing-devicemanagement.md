---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6136d83043d7c996340869d36ae63c17bdc736656a5f57de4e33e345d488b295
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155080"
---
# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune-auditing-devicemanagement-get.md)|[deviceManagement](../resources/intune-auditing-devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune-auditing-devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune-auditing-devicemanagement-update.md)|[deviceManagement](../resources/intune-auditing-devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune-auditing-devicemanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|auditEvents|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|События аудита|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




