---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e4470d1ce22f5ffbf3c805adc5328398d57d9fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056926"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="e4948-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="e4948-103">controlScore resource type</span></span>

<span data-ttu-id="e4948-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4948-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4948-105">Содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e4948-105">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="e4948-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4948-106">Properties</span></span>

|<span data-ttu-id="e4948-107">Имя</span><span class="sxs-lookup"><span data-stu-id="e4948-107">Name</span></span> |<span data-ttu-id="e4948-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4948-108">Type</span></span> |<span data-ttu-id="e4948-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4948-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="e4948-110">контролнаме</span><span class="sxs-lookup"><span data-stu-id="e4948-110">controlName</span></span>|<span data-ttu-id="e4948-111">String</span><span class="sxs-lookup"><span data-stu-id="e4948-111">String</span></span>|<span data-ttu-id="e4948-112">Уникальное имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e4948-112">Control unique name.</span></span>|
|<span data-ttu-id="e4948-113">коэффициент</span><span class="sxs-lookup"><span data-stu-id="e4948-113">score</span></span>|<span data-ttu-id="e4948-114">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="e4948-114">Double</span></span>|<span data-ttu-id="e4948-115">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="e4948-115">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="e4948-116">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="e4948-116">controlCategory</span></span>|<span data-ttu-id="e4948-117">String</span><span class="sxs-lookup"><span data-stu-id="e4948-117">String</span></span>|<span data-ttu-id="e4948-118">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="e4948-118">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="e4948-119">description</span><span class="sxs-lookup"><span data-stu-id="e4948-119">description</span></span>|<span data-ttu-id="e4948-120">String</span><span class="sxs-lookup"><span data-stu-id="e4948-120">String</span></span>| <span data-ttu-id="e4948-121">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="e4948-121">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4948-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4948-122">JSON representation</span></span>

<span data-ttu-id="e4948-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4948-123">The following is a JSON representation of the resource.</span></span>

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

