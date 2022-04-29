---
title: Тип ресурса requestSchedule
description: В PIM используйте этот ресурс, чтобы определить расписание, в течение которых субъект будет иметь допустимую или активную роль.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 67fb91da3601c467e33725064ca68753f35eab86
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134444"
---
# <a name="requestschedule-resource-type"></a>Тип ресурса requestSchedule

Пространство имен: microsoft.graph

В PIM используйте этот ресурс, чтобы определить расписание, в течение которых субъекту будет присвоено допустимое или активное назначение ролей.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Истечения срока действия|[expirationPattern](../resources/expirationpattern.md)|По истечении срока действия допустимого или активного назначения.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|Частота допустимого или активного назначения. Это свойство в настоящее время не поддерживается в PIM.|
|startDateTime|DateTimeOffset|Когда допустимое или активное назначение становится активным.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```

