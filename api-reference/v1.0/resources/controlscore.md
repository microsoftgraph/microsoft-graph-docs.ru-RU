---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68e4bf278b7d1b6ea6f00f75192847abab1ae3a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032846"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="98ea8-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="98ea8-103">controlScore resource type</span></span>

<span data-ttu-id="98ea8-104">Содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="98ea8-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="98ea8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="98ea8-105">Properties</span></span>

|<span data-ttu-id="98ea8-106">Имя</span><span class="sxs-lookup"><span data-stu-id="98ea8-106">Name</span></span> |<span data-ttu-id="98ea8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="98ea8-107">Type</span></span> |<span data-ttu-id="98ea8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="98ea8-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="98ea8-109">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="98ea8-109">controlName</span></span>|<span data-ttu-id="98ea8-110">String</span><span class="sxs-lookup"><span data-stu-id="98ea8-110">String</span></span>|<span data-ttu-id="98ea8-111">Уникальное имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="98ea8-111">Control unique name.</span></span>|
|<span data-ttu-id="98ea8-112">score</span><span class="sxs-lookup"><span data-stu-id="98ea8-112">score</span></span>|<span data-ttu-id="98ea8-113">Двойное</span><span class="sxs-lookup"><span data-stu-id="98ea8-113">Double</span></span>|<span data-ttu-id="98ea8-114">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="98ea8-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="98ea8-115">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="98ea8-115">controlCategory</span></span>|<span data-ttu-id="98ea8-116">String</span><span class="sxs-lookup"><span data-stu-id="98ea8-116">String</span></span>|<span data-ttu-id="98ea8-117">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="98ea8-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="98ea8-118">description</span><span class="sxs-lookup"><span data-stu-id="98ea8-118">description</span></span>|<span data-ttu-id="98ea8-119">String</span><span class="sxs-lookup"><span data-stu-id="98ea8-119">String</span></span>| <span data-ttu-id="98ea8-120">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="98ea8-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98ea8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98ea8-121">JSON representation</span></span>

<span data-ttu-id="98ea8-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98ea8-122">The following is a JSON representation of the resource.</span></span>

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
