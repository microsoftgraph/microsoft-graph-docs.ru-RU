---
title: " Тип ресурса controlScore"
description: Этот ресурс содержит счета клиента и описание для отдельного элемента управления.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891471"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="52f32-103">Тип ресурса controlScore</span><span class="sxs-lookup"><span data-stu-id="52f32-103">controlScore resource type</span></span>

<span data-ttu-id="52f32-104">Этот ресурс содержит счета клиента и описание для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="52f32-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="52f32-105">Имя</span><span class="sxs-lookup"><span data-stu-id="52f32-105">Name</span></span> |<span data-ttu-id="52f32-106">Тип</span><span class="sxs-lookup"><span data-stu-id="52f32-106">Type</span></span> |<span data-ttu-id="52f32-107">Описание</span><span class="sxs-lookup"><span data-stu-id="52f32-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="52f32-108">ИмяЭлементаУправления</span><span class="sxs-lookup"><span data-stu-id="52f32-108">controlName</span></span> |   <span data-ttu-id="52f32-109">Строка</span><span class="sxs-lookup"><span data-stu-id="52f32-109">String</span></span>  |   <span data-ttu-id="52f32-110">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="52f32-110">Control unique name</span></span> |
|   <span data-ttu-id="52f32-111">score</span><span class="sxs-lookup"><span data-stu-id="52f32-111">score</span></span>   |   <span data-ttu-id="52f32-112">Double</span><span class="sxs-lookup"><span data-stu-id="52f32-112">Double</span></span>  |  <span data-ttu-id="52f32-113">Клиент достичь счета для элемента управления (он зависит от дня операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="52f32-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="52f32-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="52f32-114">controlCategory</span></span> |   <span data-ttu-id="52f32-115">Строка</span><span class="sxs-lookup"><span data-stu-id="52f32-115">String</span></span>  |  <span data-ttu-id="52f32-116">Категория действие элемента управления (удостоверения, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="52f32-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="52f32-117">описание</span><span class="sxs-lookup"><span data-stu-id="52f32-117">description</span></span> |   <span data-ttu-id="52f32-118">Строка</span><span class="sxs-lookup"><span data-stu-id="52f32-118">String</span></span>  |  <span data-ttu-id="52f32-119">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="52f32-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52f32-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52f32-120">JSON representation</span></span>

<span data-ttu-id="52f32-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52f32-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "String",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
