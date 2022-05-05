---
title: Тип ресурса androidFotaDeploymentAssignmentTarget
description: Группа AAD, в которая развертываются обновления встроенного ПО
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1bc95f25abe2f1971573a4b4904b2535420fe9ff
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213312"
---
# <a name="androidfotadeploymentassignmenttarget-resource-type"></a>Тип ресурса androidFotaDeploymentAssignmentTarget

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Группа AAD, в которая развертываются обновления встроенного ПО

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|String|AAD группы.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidFotaDeploymentAssignmentTarget",
  "groupId": "String"
}
```




