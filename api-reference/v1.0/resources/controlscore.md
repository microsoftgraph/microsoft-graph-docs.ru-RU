---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629287"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="32f29-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="32f29-103">controlScore resource type</span></span>

<span data-ttu-id="32f29-104">Содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32f29-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="32f29-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="32f29-105">Properties</span></span>

|<span data-ttu-id="32f29-106">Имя</span><span class="sxs-lookup"><span data-stu-id="32f29-106">Name</span></span> |<span data-ttu-id="32f29-107">Тип</span><span class="sxs-lookup"><span data-stu-id="32f29-107">Type</span></span> |<span data-ttu-id="32f29-108">Описание</span><span class="sxs-lookup"><span data-stu-id="32f29-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="32f29-109">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="32f29-109">controlName</span></span>|<span data-ttu-id="32f29-110">String</span><span class="sxs-lookup"><span data-stu-id="32f29-110">String</span></span>|<span data-ttu-id="32f29-111">Уникальное имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32f29-111">Control unique name.</span></span>|
|<span data-ttu-id="32f29-112">score</span><span class="sxs-lookup"><span data-stu-id="32f29-112">score</span></span>|<span data-ttu-id="32f29-113">Двойное</span><span class="sxs-lookup"><span data-stu-id="32f29-113">Double</span></span>|<span data-ttu-id="32f29-114">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="32f29-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="32f29-115">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="32f29-115">controlCategory</span></span>|<span data-ttu-id="32f29-116">String</span><span class="sxs-lookup"><span data-stu-id="32f29-116">String</span></span>|<span data-ttu-id="32f29-117">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="32f29-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="32f29-118">description</span><span class="sxs-lookup"><span data-stu-id="32f29-118">description</span></span>|<span data-ttu-id="32f29-119">String</span><span class="sxs-lookup"><span data-stu-id="32f29-119">String</span></span>| <span data-ttu-id="32f29-120">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32f29-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32f29-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="32f29-121">JSON representation</span></span>

<span data-ttu-id="32f29-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32f29-122">The following is a JSON representation of the resource.</span></span>

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
