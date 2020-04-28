---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f718e197e690d3779870e5996161461fe8f60915
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507417"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="f277a-103">Тип ресурса Контролскоре</span><span class="sxs-lookup"><span data-stu-id="f277a-103">controlScore resource type</span></span>

<span data-ttu-id="f277a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f277a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f277a-105">Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f277a-105">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="f277a-106">Имя</span><span class="sxs-lookup"><span data-stu-id="f277a-106">Name</span></span> |<span data-ttu-id="f277a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f277a-107">Type</span></span> |<span data-ttu-id="f277a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f277a-108">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="f277a-109">контролнаме</span><span class="sxs-lookup"><span data-stu-id="f277a-109">controlName</span></span> |   <span data-ttu-id="f277a-110">String</span><span class="sxs-lookup"><span data-stu-id="f277a-110">String</span></span>  |   <span data-ttu-id="f277a-111">Уникальное имя элемента управления</span><span class="sxs-lookup"><span data-stu-id="f277a-111">Control unique name</span></span> |
|   <span data-ttu-id="f277a-112">коэффициент</span><span class="sxs-lookup"><span data-stu-id="f277a-112">score</span></span>   |   <span data-ttu-id="f277a-113">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="f277a-113">Double</span></span>  |  <span data-ttu-id="f277a-114">Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).</span><span class="sxs-lookup"><span data-stu-id="f277a-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="f277a-115">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="f277a-115">controlCategory</span></span> |   <span data-ttu-id="f277a-116">String</span><span class="sxs-lookup"><span data-stu-id="f277a-116">String</span></span>  |  <span data-ttu-id="f277a-117">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="f277a-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="f277a-118">description</span><span class="sxs-lookup"><span data-stu-id="f277a-118">description</span></span> |   <span data-ttu-id="f277a-119">String</span><span class="sxs-lookup"><span data-stu-id="f277a-119">String</span></span>  |  <span data-ttu-id="f277a-120">Описание элемента управления.</span><span class="sxs-lookup"><span data-stu-id="f277a-120">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f277a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f277a-121">JSON representation</span></span>

<span data-ttu-id="f277a-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f277a-122">The following is a JSON representation of the resource.</span></span>

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
