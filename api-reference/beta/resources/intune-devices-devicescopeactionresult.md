---
title: Тип ресурса deviceScopeActionResult
description: Результат активируемого действия области устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6938869b658edb1d0fddc4dfa753e45cb1fb8eb5
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858802"
---
# <a name="devicescopeactionresult-resource-type"></a>Тип ресурса deviceScopeActionResult

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Результат активируемого действия области устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceScopeAction|[deviceScopeAction](../resources/intune-devices-devicescopeaction.md)|Имя активируемого действия. Возможные значения: .|
|deviceScopeId|Строка|Уникальный идентификатор области устройства, в которой активируется действие.|
|status|[deviceScopeActionStatus](../resources/intune-devices-devicescopeactionstatus.md)|Указывает состояние действия области устройства попытки. При успешном выполнении действие было активироваться с ошибкой. В случае сбоя действие не срабатывалось. Возможные значения: `failed`, `succeeded`, `unknownFutureValue`.|
|failedMessage|String|В сообщении указывается причина, по которой не удалось активировать действие области устройства.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceScopeActionResult"
}
-->
``` json
{
  "@odata.type": "microsoft.graph.deviceScopeActionResult",
  "deviceScopeAction": "String",
  "deviceScopeId": "String",
  "status": "String",
  "failedMessage": "String"
}
```




