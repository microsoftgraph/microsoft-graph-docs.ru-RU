---
title: Тип ресурса deviceScopeActionResult
description: Результат активируемого действия области устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3f991b685f2982a4b913325f409cff34ba8a985
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670325"
---
# <a name="devicescopeactionresult-resource-type"></a>Тип ресурса deviceScopeActionResult

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Результат активируемого действия области устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceScopeAction|[deviceScopeAction](../resources/intune-devices-devicescopeaction.md)|Имя активируемого действия. Возможные значения: .|
|deviceScopeId|String|Уникальный идентификатор области устройства, в которой активируется действие.|
|status|[deviceScopeActionStatus](../resources/intune-devices-devicescopeactionstatus.md)|Указывает состояние действия области устройства попытки. При успешном выполнении действие было активироваться с ошибкой. В случае сбоя действие не срабатывалось. Возможные значения: `failed`, `succeeded`, `unknownFutureValue`.|
|failedMessage|String|В сообщении указывается причина, по которой не удалось активировать действие области устройства.|

## <a name="relationships"></a>Связи
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
  "@odata.type": "#microsoft.graph.deviceScopeActionResult",
  "deviceScopeAction": "String",
  "deviceScopeId": "String",
  "status": "String",
  "failedMessage": "String"
}
```




