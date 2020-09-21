---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3eb06ecc8937fd8f2d6c8d74cd0aaf560a22b89c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989460"
---
# <a name="macoslobchildapp-resource-type"></a>Тип ресурса Макослобчилдапп

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства бизнес-приложения MacOS в пакете набора

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleId|String|Имя удостоверения.|
|buildNumber|String|Номер сборки бизнес-приложения MacOS бизнес (LoB).|
|versionNumber|String|Номер версии приложения MacOS для бизнеса (LoB).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```






