---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
ms.openlocfilehash: 648242b827c0390029522955b0fe6347b98100c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331334"
---
# <a name="insightidentity"></a><span data-ttu-id="84973-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="84973-103">insightIdentity</span></span>

> <span data-ttu-id="84973-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84973-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84973-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84973-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84973-106">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="84973-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="84973-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84973-107">JSON representation</span></span>
<span data-ttu-id="84973-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="84973-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="84973-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="84973-109">Properties</span></span>

| <span data-ttu-id="84973-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="84973-110">Property</span></span>              | <span data-ttu-id="84973-111">Тип</span><span class="sxs-lookup"><span data-stu-id="84973-111">Type</span></span>          | <span data-ttu-id="84973-112">Описание</span><span class="sxs-lookup"><span data-stu-id="84973-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="84973-113">displayName</span><span class="sxs-lookup"><span data-stu-id="84973-113">displayName</span></span>       | <span data-ttu-id="84973-114">Строка</span><span class="sxs-lookup"><span data-stu-id="84973-114">String</span></span>          | <span data-ttu-id="84973-115">Отображаемое имя пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="84973-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="84973-116">id</span><span class="sxs-lookup"><span data-stu-id="84973-116">id</span></span>              | <span data-ttu-id="84973-117">Строка</span><span class="sxs-lookup"><span data-stu-id="84973-117">String</span></span>        | <span data-ttu-id="84973-118">Идентификатор пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="84973-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="84973-119">address</span><span class="sxs-lookup"><span data-stu-id="84973-119">address</span></span>             | <span data-ttu-id="84973-120">String</span><span class="sxs-lookup"><span data-stu-id="84973-120">String</span></span>      | <span data-ttu-id="84973-121">Адрес электронной почты пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="84973-121">The email address of the user who shared the item.</span></span>  |