---
title: Тип ресурса администрирования
description: Объект, который выступает в качестве контейнера для функций администратора.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: fbd064916aca2b0b355eadaa90f56bc2186638ce
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447079"
---
# <a name="admin-resource-type"></a>Тип ресурса администрирования

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, который выступает в качестве контейнера для функций администратора.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
| serviceAnnouncement | [serviceAnnouncement](serviceannouncement.md) | Контейнер для ресурсов связи службы. Только для чтения. |
|Windows|[microsoft.graph.windowsUpdates.windows](../resources/windowsupdates-windows.md)|Контейнер для всех Windows обновления для службы развертывания бизнеса. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.admin",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.admin"
}
```

