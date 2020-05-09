---
title: Тип ресурса Макоссистемекстенсионтипемаппинг
description: Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3422cdac178ba22dee07aadb4700e2806eedc7ba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179392"
---
# <a name="macossystemextensiontypemapping-resource-type"></a>Тип ресурса Макоссистемекстенсионтипемаппинг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|теамидентифиер|Строка|Получает или задает идентификатор группы, используемый для подписи расширения системы.|
|алловедтипес|[макоссистемекстенсионтипе](../resources/intune-deviceconfig-macossystemextensiontype.md)|Получает или задает разрешенные типы расширений системы macOS. Возможные значения: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtensionTypeMapping",
  "teamIdentifier": "String",
  "allowedTypes": "String"
}
```



