---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc3de6363784f62792d7c4e56906c79ed1be0c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531767"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="0f5cb-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="0f5cb-103">controlScore resource type</span></span>

<span data-ttu-id="0f5cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f5cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f5cb-105">Содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="0f5cb-105">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="0f5cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f5cb-106">Properties</span></span>

|<span data-ttu-id="0f5cb-107">Имя</span><span class="sxs-lookup"><span data-stu-id="0f5cb-107">Name</span></span> |<span data-ttu-id="0f5cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f5cb-108">Type</span></span> |<span data-ttu-id="0f5cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f5cb-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="0f5cb-110">контролнаме</span><span class="sxs-lookup"><span data-stu-id="0f5cb-110">controlName</span></span>|<span data-ttu-id="0f5cb-111">String</span><span class="sxs-lookup"><span data-stu-id="0f5cb-111">String</span></span>|<span data-ttu-id="0f5cb-112">Уникальное имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="0f5cb-112">Control unique name.</span></span>|
|<span data-ttu-id="0f5cb-113">коэффициент</span><span class="sxs-lookup"><span data-stu-id="0f5cb-113">score</span></span>|<span data-ttu-id="0f5cb-114">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0f5cb-114">Double</span></span>|<span data-ttu-id="0f5cb-115">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="0f5cb-115">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="0f5cb-116">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="0f5cb-116">controlCategory</span></span>|<span data-ttu-id="0f5cb-117">String</span><span class="sxs-lookup"><span data-stu-id="0f5cb-117">String</span></span>|<span data-ttu-id="0f5cb-118">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="0f5cb-118">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="0f5cb-119">description</span><span class="sxs-lookup"><span data-stu-id="0f5cb-119">description</span></span>|<span data-ttu-id="0f5cb-120">String</span><span class="sxs-lookup"><span data-stu-id="0f5cb-120">String</span></span>| <span data-ttu-id="0f5cb-121">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="0f5cb-121">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f5cb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f5cb-122">JSON representation</span></span>

<span data-ttu-id="0f5cb-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f5cb-123">The following is a JSON representation of the resource.</span></span>

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
