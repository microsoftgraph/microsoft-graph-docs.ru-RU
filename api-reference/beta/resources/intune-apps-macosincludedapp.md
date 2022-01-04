---
title: тип ресурса macOSIncludedApp
description: Содержит свойства включенного приложения .app в приложении MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87c7d8b5cc5eb1229b9860fe8192b0cd765c33c5
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712230"
---
# <a name="macosincludedapp-resource-type"></a>тип ресурса macOSIncludedApp

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства включенного приложения .app в приложении MacOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleId|String|The CFBundleIdentifier.|
|bundleVersion|String|The CFBundleVersion.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSIncludedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSIncludedApp",
  "bundleId": "String",
  "bundleVersion": "String"
}
```




