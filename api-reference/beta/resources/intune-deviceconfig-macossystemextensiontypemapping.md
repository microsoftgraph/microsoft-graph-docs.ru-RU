---
title: Тип ресурса Макоссистемекстенсионтипемаппинг
description: Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd22cc58d3d949c1e560d62e672e27fb31ae913e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279782"
---
# <a name="macossystemextensiontypemapping-resource-type"></a>Тип ресурса Макоссистемекстенсионтипемаппинг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|теамидентифиер|String|Получает или задает идентификатор группы, используемый для подписи расширения системы.|
|алловедтипес|[macOSSystemExtensionType](../resources/intune-deviceconfig-macossystemextensiontype.md)|Получает или задает разрешенные типы расширений системы macOS. Возможные значения: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.|

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




