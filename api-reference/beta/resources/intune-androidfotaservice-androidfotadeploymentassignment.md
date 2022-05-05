---
title: Тип ресурса androidFotaDeploymentAssignment
description: Описывает группу безопасности развертывания для назначения развертывания. Серверная часть раскроет идентификатор группы безопасности, чтобы извлечь серийные номера устройств перед отправкой запроса на создание развертывания в Zebra.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c159840ba5bb2035223a45f0dec54a94055a2176
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213554"
---
# <a name="androidfotadeploymentassignment-resource-type"></a>Тип ресурса androidFotaDeploymentAssignment

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает группу безопасности развертывания для назначения развертывания. Серверная часть раскроет идентификатор группы безопасности, чтобы извлечь серийные номера устройств перед отправкой запроса на создание развертывания в Zebra.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка| Ключ для сущности назначения FOTA для Android|
|target|[androidFotaDeploymentAssignmentTarget](../resources/intune-androidfotaservice-androidfotadeploymentassignmenttarget.md)|Группа AAD, в которая развертываются обновления встроенного ПО|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidFotaDeploymentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
    "groupId": "String"
  }
}
```




