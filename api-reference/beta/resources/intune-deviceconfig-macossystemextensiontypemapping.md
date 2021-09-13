---
title: тип ресурса macOSSystemExtensionTypeMapping
description: Представляет сопоставление между идентификаторами группы для расширений системы macOS и типами расширения системы.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc2ff377d081c478a23f419c29b3f773f0c9c021
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59131289"
---
# <a name="macossystemextensiontypemapping-resource-type"></a>тип ресурса macOSSystemExtensionTypeMapping

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сопоставление между идентификаторами группы для расширений системы macOS и типами расширения системы.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|teamIdentifier|String|Получает или задает идентификатор группы, используемый для подписи расширения системы.|
|allowedTypes|[macOSSystemExtensionType](../resources/intune-deviceconfig-macossystemextensiontype.md)|Получает или задает допустимые типы расширения системы macOS. Возможные значения: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.|

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



