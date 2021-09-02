---
title: тип ресурса deviceManagementSettingCollectionConstraint
description: Ограничение, которое обеспечивает максимальное количество элементов коллекции
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9d4a342f5ccbe3fa4ec1564833037be00b76861
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819103"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a>тип ресурса deviceManagementSettingCollectionConstraint

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, которое обеспечивает максимальное количество элементов коллекции


Наследует [от deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|minimumLength|Int32|Минимальное количество элементов в коллекции|
|maximumLength|Int32|Максимальное количество элементов в коллекции|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingCollectionConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCollectionConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



