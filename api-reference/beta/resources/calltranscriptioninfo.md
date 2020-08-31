---
title: Тип ресурса Каллтранскриптионинфо
description: Представляет одно событие DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f2f91b8aadfd9f819e87eff839090aa37166cf2
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312215"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="adf89-103">Тип ресурса Каллтранскриптионинфо</span><span class="sxs-lookup"><span data-stu-id="adf89-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="adf89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adf89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adf89-105">Представляет одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="adf89-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="adf89-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="adf89-106">Properties</span></span>

| <span data-ttu-id="adf89-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="adf89-107">Property</span></span>       | <span data-ttu-id="adf89-108">Тип</span><span class="sxs-lookup"><span data-stu-id="adf89-108">Type</span></span>    | <span data-ttu-id="adf89-109">Описание</span><span class="sxs-lookup"><span data-stu-id="adf89-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="adf89-110">state</span><span class="sxs-lookup"><span data-stu-id="adf89-110">state</span></span> | <span data-ttu-id="adf89-111">String</span><span class="sxs-lookup"><span data-stu-id="adf89-111">String</span></span> | <span data-ttu-id="adf89-112">Возможные значения: `notStarted`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="adf89-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="adf89-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adf89-113">lastModifiedDateTime</span></span> | <span data-ttu-id="adf89-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="adf89-114">DateTime</span></span> | <span data-ttu-id="adf89-115">Время изменения состояния в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="adf89-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="adf89-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adf89-116">JSON representation</span></span>

<span data-ttu-id="adf89-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adf89-117">The following is a JSON representation of the resource.</span></span>

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
