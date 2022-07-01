---
title: Тип ресурса synchronizationLinkedObjects
description: Представляет все ссылки, которые необходимо подготовить во время подготовки по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 27053821607e8a813c690e18aa658256c0ff1038
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447770"
---
# <a name="synchronizationlinkedobjects-resource-type"></a>Тип ресурса synchronizationLinkedObjects

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет все ссылки, которые необходимо подготовить во время подготовки по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|members|[Коллекция synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)|Все участники группы, которые вы хотите подготовить.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationLinkedObjects"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationLinkedObjects",
  "members": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```
