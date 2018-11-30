---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
ms.openlocfilehash: c0e340374b9dfc43b80fa310923785c0475a9532
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078828"
---
# <a name="appconfigurationsettingitem-resource-type"></a>Тип ресурса appConfigurationSettingItem

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для элемента параметра конфигурации приложения.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appConfigKey|Строка|Ключ конфигурации приложения.|
|appConfigKeyType|[mdmAppConfigKeyType](../resources/intune-apps-mdmappconfigkeytype.md)|Тип ключа конфигурации приложения. Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.|
|appConfigKeyValue|Строка|Значение ключа конфигурации приложения.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```





