---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 395c865a38ebe6ea84dc64857f441cd529e4f2d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886578"
---
# <a name="insightidentity"></a><span data-ttu-id="bf2e9-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="bf2e9-103">insightIdentity</span></span>

> <span data-ttu-id="bf2e9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf2e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf2e9-106">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bf2e9-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf2e9-107">JSON representation</span></span>
<span data-ttu-id="bf2e9-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="bf2e9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf2e9-109">Properties</span></span>

| <span data-ttu-id="bf2e9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf2e9-110">Property</span></span>              | <span data-ttu-id="bf2e9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bf2e9-111">Type</span></span>          | <span data-ttu-id="bf2e9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2e9-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="bf2e9-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bf2e9-113">displayName</span></span>       | <span data-ttu-id="bf2e9-114">Строка</span><span class="sxs-lookup"><span data-stu-id="bf2e9-114">String</span></span>          | <span data-ttu-id="bf2e9-115">Отображаемое имя пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="bf2e9-116">id</span><span class="sxs-lookup"><span data-stu-id="bf2e9-116">id</span></span>              | <span data-ttu-id="bf2e9-117">Строка</span><span class="sxs-lookup"><span data-stu-id="bf2e9-117">String</span></span>        | <span data-ttu-id="bf2e9-118">Идентификатор пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="bf2e9-119">address</span><span class="sxs-lookup"><span data-stu-id="bf2e9-119">address</span></span>             | <span data-ttu-id="bf2e9-120">String</span><span class="sxs-lookup"><span data-stu-id="bf2e9-120">String</span></span>      | <span data-ttu-id="bf2e9-121">Адрес электронной почты пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="bf2e9-121">The email address of the user who shared the item.</span></span>  |
