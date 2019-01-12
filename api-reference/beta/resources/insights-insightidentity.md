---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a263caa68280128a67a027b75682407fd4932605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938939"
---
# <a name="insightidentity"></a><span data-ttu-id="96e22-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="96e22-103">insightIdentity</span></span>

> <span data-ttu-id="96e22-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96e22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96e22-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96e22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96e22-106">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="96e22-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="96e22-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96e22-107">JSON representation</span></span>
<span data-ttu-id="96e22-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="96e22-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="96e22-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="96e22-109">Properties</span></span>

| <span data-ttu-id="96e22-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="96e22-110">Property</span></span>              | <span data-ttu-id="96e22-111">Тип</span><span class="sxs-lookup"><span data-stu-id="96e22-111">Type</span></span>          | <span data-ttu-id="96e22-112">Описание</span><span class="sxs-lookup"><span data-stu-id="96e22-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="96e22-113">displayName</span><span class="sxs-lookup"><span data-stu-id="96e22-113">displayName</span></span>       | <span data-ttu-id="96e22-114">Строка</span><span class="sxs-lookup"><span data-stu-id="96e22-114">String</span></span>          | <span data-ttu-id="96e22-115">Отображаемое имя пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="96e22-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="96e22-116">id</span><span class="sxs-lookup"><span data-stu-id="96e22-116">id</span></span>              | <span data-ttu-id="96e22-117">Строка</span><span class="sxs-lookup"><span data-stu-id="96e22-117">String</span></span>        | <span data-ttu-id="96e22-118">Идентификатор пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="96e22-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="96e22-119">address</span><span class="sxs-lookup"><span data-stu-id="96e22-119">address</span></span>             | <span data-ttu-id="96e22-120">String</span><span class="sxs-lookup"><span data-stu-id="96e22-120">String</span></span>      | <span data-ttu-id="96e22-121">Адрес электронной почты пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="96e22-121">The email address of the user who shared the item.</span></span>  |
