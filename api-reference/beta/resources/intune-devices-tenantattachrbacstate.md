---
title: тип ресурса tenantAttachRBACState
description: Представляет результат API GetState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 534570f827eb96658f49f115e6a5d3ba5bdc7d26
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631364"
---
# <a name="tenantattachrbacstate-resource-type"></a>тип ресурса tenantAttachRBACState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет результат API GetState.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enabled|Boolean|Указывает, включен ли клиент для tenant Attach с управлением ролью.  TRUE, если включено, FALSE, если присоединение клиента с функцией rolemanagement отключено.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tenantAttachRBACState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantAttachRBACState",
  "enabled": true
}
```




