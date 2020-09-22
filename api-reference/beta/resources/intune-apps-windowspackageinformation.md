---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d743454f5b0acfa9a8ba6c1b205d67fcb3c11595
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070921"
---
# <a name="windowspackageinformation-resource-type"></a>Тип ресурса windowsPackageInformation

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сведений о пакете для бизнес-приложения Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Архитектура Windows, в которой можно запустить это приложение. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|displayName|String|Отображаемое имя.|
|identityName|String|Имя удостоверения.|
|идентитипублишер|String|Издатель удостоверений.|
|identityResourceIdentifier|String|Идентификатор ресурса Identity.|
|identityVersion|String|Версия идентификатора.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  }
}
```






