---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 89e448d828f1f7caef73b14586b06d1df238f100
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973935"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="0bfd9-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="0bfd9-103">controlScore resource type</span></span>

<span data-ttu-id="0bfd9-104">Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="0bfd9-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="0bfd9-105">Имя</span><span class="sxs-lookup"><span data-stu-id="0bfd9-105">Name</span></span> |<span data-ttu-id="0bfd9-106">Тип</span><span class="sxs-lookup"><span data-stu-id="0bfd9-106">Type</span></span> |<span data-ttu-id="0bfd9-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0bfd9-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="0bfd9-108">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="0bfd9-108">controlName</span></span> |   <span data-ttu-id="0bfd9-109">String</span><span class="sxs-lookup"><span data-stu-id="0bfd9-109">String</span></span>  |   <span data-ttu-id="0bfd9-110">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="0bfd9-110">Control unique name</span></span> |
|   <span data-ttu-id="0bfd9-111">score</span><span class="sxs-lookup"><span data-stu-id="0bfd9-111">score</span></span>   |   <span data-ttu-id="0bfd9-112">Двойное</span><span class="sxs-lookup"><span data-stu-id="0bfd9-112">Double</span></span>  |  <span data-ttu-id="0bfd9-113">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="0bfd9-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="0bfd9-114">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="0bfd9-114">controlCategory</span></span> |   <span data-ttu-id="0bfd9-115">String</span><span class="sxs-lookup"><span data-stu-id="0bfd9-115">String</span></span>  |  <span data-ttu-id="0bfd9-116">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="0bfd9-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="0bfd9-117">description</span><span class="sxs-lookup"><span data-stu-id="0bfd9-117">description</span></span> |   <span data-ttu-id="0bfd9-118">String</span><span class="sxs-lookup"><span data-stu-id="0bfd9-118">String</span></span>  |  <span data-ttu-id="0bfd9-119">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="0bfd9-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0bfd9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bfd9-120">JSON representation</span></span>

<span data-ttu-id="0bfd9-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bfd9-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
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
