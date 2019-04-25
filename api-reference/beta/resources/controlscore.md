---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543380"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="61c55-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="61c55-103">controlScore resource type</span></span>

<span data-ttu-id="61c55-104">Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="61c55-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="61c55-105">Имя</span><span class="sxs-lookup"><span data-stu-id="61c55-105">Name</span></span> |<span data-ttu-id="61c55-106">Тип</span><span class="sxs-lookup"><span data-stu-id="61c55-106">Type</span></span> |<span data-ttu-id="61c55-107">Описание</span><span class="sxs-lookup"><span data-stu-id="61c55-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="61c55-108">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="61c55-108">controlName</span></span> |   <span data-ttu-id="61c55-109">String</span><span class="sxs-lookup"><span data-stu-id="61c55-109">String</span></span>  |   <span data-ttu-id="61c55-110">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="61c55-110">Control unique name</span></span> |
|   <span data-ttu-id="61c55-111">score</span><span class="sxs-lookup"><span data-stu-id="61c55-111">score</span></span>   |   <span data-ttu-id="61c55-112">Двойное</span><span class="sxs-lookup"><span data-stu-id="61c55-112">Double</span></span>  |  <span data-ttu-id="61c55-113">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="61c55-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="61c55-114">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="61c55-114">controlCategory</span></span> |   <span data-ttu-id="61c55-115">String</span><span class="sxs-lookup"><span data-stu-id="61c55-115">String</span></span>  |  <span data-ttu-id="61c55-116">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="61c55-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="61c55-117">description</span><span class="sxs-lookup"><span data-stu-id="61c55-117">description</span></span> |   <span data-ttu-id="61c55-118">String</span><span class="sxs-lookup"><span data-stu-id="61c55-118">String</span></span>  |  <span data-ttu-id="61c55-119">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="61c55-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61c55-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="61c55-120">JSON representation</span></span>

<span data-ttu-id="61c55-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61c55-121">The following is a JSON representation of the resource.</span></span>

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
