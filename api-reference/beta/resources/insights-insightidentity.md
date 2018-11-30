---
title: insightIdentity
description: " Тип ресурса"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079417"
---
# <a name="insightidentity"></a><span data-ttu-id="cc6fc-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="cc6fc-103">insightIdentity</span></span>

> <span data-ttu-id="cc6fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc6fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-105">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="cc6fc-106">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="cc6fc-106">resource type</span></span>

<span data-ttu-id="cc6fc-107">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-107">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="cc6fc-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc6fc-108">JSON representation</span></span>
<span data-ttu-id="cc6fc-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-109">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="cc6fc-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc6fc-110">Properties</span></span>

| <span data-ttu-id="cc6fc-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc6fc-111">Property</span></span>              | <span data-ttu-id="cc6fc-112">Тип</span><span class="sxs-lookup"><span data-stu-id="cc6fc-112">Type</span></span>          | <span data-ttu-id="cc6fc-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cc6fc-113">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="cc6fc-114">displayName</span><span class="sxs-lookup"><span data-stu-id="cc6fc-114">displayName</span></span>       | <span data-ttu-id="cc6fc-115">String</span><span class="sxs-lookup"><span data-stu-id="cc6fc-115">String</span></span>          | <span data-ttu-id="cc6fc-116">Отображаемое имя пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-116">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="cc6fc-117">id</span><span class="sxs-lookup"><span data-stu-id="cc6fc-117">id</span></span>              | <span data-ttu-id="cc6fc-118">String</span><span class="sxs-lookup"><span data-stu-id="cc6fc-118">String</span></span>        | <span data-ttu-id="cc6fc-119">Идентификатор пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-119">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="cc6fc-120">address</span><span class="sxs-lookup"><span data-stu-id="cc6fc-120">address</span></span>             | <span data-ttu-id="cc6fc-121">String</span><span class="sxs-lookup"><span data-stu-id="cc6fc-121">String</span></span>      | <span data-ttu-id="cc6fc-122">Адрес электронной почты пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="cc6fc-122">The email address of the user who shared the item.</span></span>  |