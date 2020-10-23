---
title: Тип ресурса win32LobAppRule
description: Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec25bb546cb38213f59f9a3ebece71de5db5e336
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706116"
---
# <a name="win32lobapprule-resource-type"></a>Тип ресурса win32LobAppRule

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий назначение правила. Возможные значения: `detection`, `requirement`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRule",
  "ruleType": "String"
}
```





