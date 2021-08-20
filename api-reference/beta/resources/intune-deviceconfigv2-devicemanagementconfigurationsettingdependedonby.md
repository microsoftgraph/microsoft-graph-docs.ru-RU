---
title: тип ресурса deviceManagementConfigurationSettingDependedOnBy
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a82dc6f1c690ba745d29c042b7eb428adaf1c8dfd3339dfbadff45fd66588e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227395"
---
# <a name="devicemanagementconfigurationsettingdependedonby-resource-type"></a>тип ресурса deviceManagementConfigurationSettingDependedOnBy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dependedOnBy|Строка|Идентификатор параметра ребенка, который зависит от текущего параметра|
|Обязательный|Логический|Значение, определяее, требуется ли параметр ребенка на основе выбора родительского параметра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
  "dependedOnBy": "String",
  "required": true
}
```




