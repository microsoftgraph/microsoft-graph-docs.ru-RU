---
title: " Тип ресурса controlScore"
description: Этот ресурс содержит счета клиента и описание для отдельного элемента управления.
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076142"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="5364e-103">Тип ресурса controlScore</span><span class="sxs-lookup"><span data-stu-id="5364e-103">controlScore resource type</span></span>

<span data-ttu-id="5364e-104">Этот ресурс содержит счета клиента и описание для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5364e-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="5364e-105">Имя</span><span class="sxs-lookup"><span data-stu-id="5364e-105">Name</span></span> |<span data-ttu-id="5364e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="5364e-106">Type</span></span> |<span data-ttu-id="5364e-107">Description</span><span class="sxs-lookup"><span data-stu-id="5364e-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="5364e-108">ИмяЭлементаУправления</span><span class="sxs-lookup"><span data-stu-id="5364e-108">controlName</span></span> |   <span data-ttu-id="5364e-109">String</span><span class="sxs-lookup"><span data-stu-id="5364e-109">String</span></span>  |   <span data-ttu-id="5364e-110">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="5364e-110">Control unique name</span></span> |
|   <span data-ttu-id="5364e-111">score</span><span class="sxs-lookup"><span data-stu-id="5364e-111">score</span></span>   |   <span data-ttu-id="5364e-112">Double</span><span class="sxs-lookup"><span data-stu-id="5364e-112">Double</span></span>  |  <span data-ttu-id="5364e-113">Клиент достичь счета для элемента управления (он зависит от дня операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="5364e-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="5364e-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="5364e-114">controlCategory</span></span> |   <span data-ttu-id="5364e-115">String</span><span class="sxs-lookup"><span data-stu-id="5364e-115">String</span></span>  |  <span data-ttu-id="5364e-116">Категория действие элемента управления (удостоверения, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="5364e-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="5364e-117">описание</span><span class="sxs-lookup"><span data-stu-id="5364e-117">description</span></span> |   <span data-ttu-id="5364e-118">String</span><span class="sxs-lookup"><span data-stu-id="5364e-118">String</span></span>  |  <span data-ttu-id="5364e-119">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="5364e-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5364e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5364e-120">JSON representation</span></span>

<span data-ttu-id="5364e-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5364e-121">The following is a JSON representation of the resource.</span></span>

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
