---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341185"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="ade71-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="ade71-103">controlScore resource type</span></span>

<span data-ttu-id="ade71-104">Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="ade71-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="ade71-105">Имя</span><span class="sxs-lookup"><span data-stu-id="ade71-105">Name</span></span> |<span data-ttu-id="ade71-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ade71-106">Type</span></span> |<span data-ttu-id="ade71-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ade71-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ade71-108">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="ade71-108">controlName</span></span> |   <span data-ttu-id="ade71-109">String</span><span class="sxs-lookup"><span data-stu-id="ade71-109">String</span></span>  |   <span data-ttu-id="ade71-110">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="ade71-110">Control unique name</span></span> |
|   <span data-ttu-id="ade71-111">score</span><span class="sxs-lookup"><span data-stu-id="ade71-111">score</span></span>   |   <span data-ttu-id="ade71-112">Двойное</span><span class="sxs-lookup"><span data-stu-id="ade71-112">Double</span></span>  |  <span data-ttu-id="ade71-113">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="ade71-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="ade71-114">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="ade71-114">controlCategory</span></span> |   <span data-ttu-id="ade71-115">String</span><span class="sxs-lookup"><span data-stu-id="ade71-115">String</span></span>  |  <span data-ttu-id="ade71-116">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="ade71-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="ade71-117">description</span><span class="sxs-lookup"><span data-stu-id="ade71-117">description</span></span> |   <span data-ttu-id="ade71-118">String</span><span class="sxs-lookup"><span data-stu-id="ade71-118">String</span></span>  |  <span data-ttu-id="ade71-119">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="ade71-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ade71-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ade71-120">JSON representation</span></span>

<span data-ttu-id="ade71-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ade71-121">The following is a JSON representation of the resource.</span></span>

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
