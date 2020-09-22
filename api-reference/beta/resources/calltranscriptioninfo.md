---
title: Тип ресурса Каллтранскриптионинфо
description: Представляет одно событие DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd95ebf165bad8cde296d54e5b0a06f969f1c903
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042711"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="05f3a-103">Тип ресурса Каллтранскриптионинфо</span><span class="sxs-lookup"><span data-stu-id="05f3a-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="05f3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05f3a-105">Представляет одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="05f3a-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="05f3a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="05f3a-106">Properties</span></span>

| <span data-ttu-id="05f3a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="05f3a-107">Property</span></span>       | <span data-ttu-id="05f3a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="05f3a-108">Type</span></span>    | <span data-ttu-id="05f3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="05f3a-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05f3a-110">state</span><span class="sxs-lookup"><span data-stu-id="05f3a-110">state</span></span> | <span data-ttu-id="05f3a-111">String</span><span class="sxs-lookup"><span data-stu-id="05f3a-111">String</span></span> | <span data-ttu-id="05f3a-112">Возможные значения: `notStarted`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="05f3a-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="05f3a-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05f3a-113">lastModifiedDateTime</span></span> | <span data-ttu-id="05f3a-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="05f3a-114">DateTime</span></span> | <span data-ttu-id="05f3a-115">Время изменения состояния в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="05f3a-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05f3a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05f3a-116">JSON representation</span></span>

<span data-ttu-id="05f3a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05f3a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callTranscriptionInfo"
}-->
```json
{
  "state": "notStarted | active | inactive",
  "lastModifiedDateTime": "String (timestamp)"
}
```


