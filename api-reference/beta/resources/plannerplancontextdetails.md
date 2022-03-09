---
title: тип ресурса plannerPlanContextDetails
description: Ресурс **plannerPlanContextDetails содержит** дополнительные сведения о планировщикеPlanContext.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bdb65fab6aecf9c61e066c7e80e9226220c3491c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367925"
---
# <a name="plannerplancontextdetails-resource-type"></a>тип ресурса plannerPlanContextDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **plannerPlanContextDetails содержит** дополнительные сведения о [планировщикеPlanContext](plannerplancontext.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customLinkText|String|Допускается значение null. Указывает текст, который используется в пользовательском интерфейсе для отображения ссылки связанного [планировщикаPlanContext](plannerplancontext.md). Если null, приложения должны отображать ссылку с пользовательским текстом на основе **свойства displayLinkType** .|
|displayLinkType|plannerPlanContextType|Указывает, как приложение должно отображать ссылку на связанный **планировщикPlanContext**. Приложения могут предоставлять настраиваемый текст, описание, значки или другие функции в зависимости от типа ссылки. Возможные значения: `teamsTab`, `sharePointPage`, `meetingNotes`, `other`, `unknownFutureValue`.|
|url|String|URL-адрес пользовательского интерфейса, представленного связанным **планировщикомPlanContext**. |
|state|plannerContextState| Указывает состояние связанного **планировщикаPlanContext**. |

### <a name="plannercontextstate-values"></a>значения plannerContextState

|Значение              |Описание|
|:------------------|:----------------------------------------------------------------------|
|active             | Контекст не имеет проблем.                                          |
|delinked           | Ранее связанный **планировщикPlanContext** больше не связан с планом. |
|unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать.                     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "string",
  "customLinkText": "string",
  "displayLinkType": "string",
  "state": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


