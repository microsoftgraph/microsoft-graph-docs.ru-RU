---
title: Тип ресурса FilterCriteria
description: Представляет условия фильтра, применяемые к столбцу.
ms.openlocfilehash: dbcc57ff940fec525b712eb11ac44209f5f8a4d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075506"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="9027a-103">Тип ресурса FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="9027a-103">FilterCriteria resource type</span></span>

> <span data-ttu-id="9027a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9027a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9027a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9027a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9027a-106">Представляет условия фильтра, применяемые к столбцу.</span><span class="sxs-lookup"><span data-stu-id="9027a-106">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9027a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9027a-107">JSON representation</span></span>

<span data-ttu-id="9027a-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9027a-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```