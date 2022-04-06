---
title: accessPackageAssignmentApprovalSettings сложный тип
description: Указывает параметры утверждения запроса на назначение пакета доступа в политике назначения пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5109cdd2482c43188409f891f782179bc1a39ebb
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608392"
---
# <a name="accesspackageassignmentapprovalsettings-complex-type"></a>accessPackageAssignmentApprovalSettings сложный тип

Пространство имен: microsoft.graph

Используется для **свойства requestApprovalSettings** политики назначения пакета [доступа](accesspackageassignmentpolicy.md). Предоставляет дополнительные параметры, чтобы указать, требуется ли утверждение для новых запросов на назначение пакета доступа через эту политику или обновления существующих запросов, а также выбрать, кто должен утвердить каждый запрос.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isApprovalRequiredForAdd|Boolean|Если `false,` в этой политике не требуется утверждение новых запросов.|
|isApprovalRequiredForUpdate|Boolean|Если `false`для обновления запросов в этой политике не требуется утверждение.|
|stages|[коллекция accessPackageApprovalStage](../resources/accesspackageapprovalstage.md)|Если требуется утверждение, один, два или три элемента этой коллекции определяют каждый из этапов утверждения. Пустой массив присутствует, если не требуется утверждение.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentApprovalSettings",
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "stages": [
    {
      "@odata.type": "microsoft.graph.accessPackageApprovalStage"
    }
  ]
}
```


