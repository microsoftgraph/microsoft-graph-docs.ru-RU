---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2b718851d1a27c3317a0ce77554be7ea3f8906a4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811499"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="3d171-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="3d171-103">controlScore resource type</span></span>

<span data-ttu-id="3d171-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d171-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d171-105">Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="3d171-105">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="3d171-106">Имя</span><span class="sxs-lookup"><span data-stu-id="3d171-106">Name</span></span> |<span data-ttu-id="3d171-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3d171-107">Type</span></span> |<span data-ttu-id="3d171-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3d171-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="3d171-109">контролнаме</span><span class="sxs-lookup"><span data-stu-id="3d171-109">controlName</span></span> |   <span data-ttu-id="3d171-110">String</span><span class="sxs-lookup"><span data-stu-id="3d171-110">String</span></span>  |   <span data-ttu-id="3d171-111">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="3d171-111">Control unique name</span></span> |
|   <span data-ttu-id="3d171-112">коэффициент</span><span class="sxs-lookup"><span data-stu-id="3d171-112">score</span></span>   |   <span data-ttu-id="3d171-113">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="3d171-113">Double</span></span>  |  <span data-ttu-id="3d171-114">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="3d171-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="3d171-115">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="3d171-115">controlCategory</span></span> |   <span data-ttu-id="3d171-116">String</span><span class="sxs-lookup"><span data-stu-id="3d171-116">String</span></span>  |  <span data-ttu-id="3d171-117">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="3d171-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="3d171-118">description</span><span class="sxs-lookup"><span data-stu-id="3d171-118">description</span></span> |   <span data-ttu-id="3d171-119">String</span><span class="sxs-lookup"><span data-stu-id="3d171-119">String</span></span>  |  <span data-ttu-id="3d171-120">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="3d171-120">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d171-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3d171-121">JSON representation</span></span>

<span data-ttu-id="3d171-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d171-122">The following is a JSON representation of the resource.</span></span>

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
