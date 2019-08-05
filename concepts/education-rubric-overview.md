---
title: Обзор рубрик в образовании
description: Рубрики — эффективный и широко применяемый способ оценки выполненных заданий, и API для образования в Microsoft Graph поддерживает их.
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: 56b9bcdf32036361fb92fe372952c94d09d8dc57
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173085"
---
# <a name="education-rubric-overview"></a><span data-ttu-id="a79ab-103">Обзор рубрик в образовании</span><span class="sxs-lookup"><span data-stu-id="a79ab-103">Education rubric overview</span></span>

<span data-ttu-id="a79ab-104">Рубрики — эффективный и широко применяемый способ оценки выполненных заданий, и API для образования в Microsoft Graph поддерживает их.</span><span class="sxs-lookup"><span data-stu-id="a79ab-104">Rubrics are an effective and widely-used way of grading assignments, and the education API in Microsoft Graph supports them.</span></span>

<span data-ttu-id="a79ab-105">Рубрика для оценивания — это матрица из*качеств*, *уровней* и *критериев*, сочетающихся следующим образом:</span><span class="sxs-lookup"><span data-stu-id="a79ab-105">A grading rubric is a matrix of *qualities*, *levels*, and *criteria*, as follows:</span></span>

| | <span data-ttu-id="a79ab-106">Уровень</span><span class="sxs-lookup"><span data-stu-id="a79ab-106">Level</span></span> | <span data-ttu-id="a79ab-107">Уровень</span><span class="sxs-lookup"><span data-stu-id="a79ab-107">Level</span></span> |
|:--|:--|:--|
| <span data-ttu-id="a79ab-108">Качество</span><span class="sxs-lookup"><span data-stu-id="a79ab-108">Print Quality</span></span> | <span data-ttu-id="a79ab-109">Критерий</span><span class="sxs-lookup"><span data-stu-id="a79ab-109">Criterion</span></span> | <span data-ttu-id="a79ab-110">Критерий</span><span class="sxs-lookup"><span data-stu-id="a79ab-110">Criterion</span></span> |
| <span data-ttu-id="a79ab-111">Качество</span><span class="sxs-lookup"><span data-stu-id="a79ab-111">Print Quality</span></span> | <span data-ttu-id="a79ab-112">Критерий</span><span class="sxs-lookup"><span data-stu-id="a79ab-112">Criterion</span></span> | <span data-ttu-id="a79ab-113">Критерий</span><span class="sxs-lookup"><span data-stu-id="a79ab-113">Criterion</span></span> |

<span data-ttu-id="a79ab-114">Пример рубрики для оценивания:</span><span class="sxs-lookup"><span data-stu-id="a79ab-114">An example of a grading rubric might be:</span></span>

| | <span data-ttu-id="a79ab-115">Хорошо</span><span class="sxs-lookup"><span data-stu-id="a79ab-115">Good</span></span> | <span data-ttu-id="a79ab-116">Плохо</span><span class="sxs-lookup"><span data-stu-id="a79ab-116">Poor</span></span> |
|:--|:--|:--|
| <span data-ttu-id="a79ab-117">Аргументация</span><span class="sxs-lookup"><span data-stu-id="a79ab-117">Argument</span></span> | <span data-ttu-id="a79ab-118">Аргументы в сочинении убедительные.</span><span class="sxs-lookup"><span data-stu-id="a79ab-118">The essay's argument is persuasive.</span></span> | <span data-ttu-id="a79ab-119">Аргументы в сочинении не имеют смысла.</span><span class="sxs-lookup"><span data-stu-id="a79ab-119">The essay's argument does not make sense.</span></span> |
| <span data-ttu-id="a79ab-120">Правописание и грамматика</span><span class="sxs-lookup"><span data-stu-id="a79ab-120">Tools > Spelling and Grammar </span></span> | <span data-ttu-id="a79ab-121">В сочинении соблюдены орфографические и грамматические нормы. Ошибок немного или вообще нет.</span><span class="sxs-lookup"><span data-stu-id="a79ab-121">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="a79ab-122">В сочинении много орфографических и грамматических ошибок.</span><span class="sxs-lookup"><span data-stu-id="a79ab-122">The essay has numerous errors in spelling and/or grammar.</span></span> |

<span data-ttu-id="a79ab-123">Оценивание посредством рубрики подразумевает выбор одного *уровня* для каждого *качества*.</span><span class="sxs-lookup"><span data-stu-id="a79ab-123">Grading using a rubric involves selecting one *level* for each *quality* in the rubric.</span></span>

<span data-ttu-id="a79ab-124">В рубрике *можно* предусматривать баллы для каждого из уровней и вес для каждого качества.</span><span class="sxs-lookup"><span data-stu-id="a79ab-124">A rubric *may* have points associated with each level, and a weight associated with each quality.</span></span>  <span data-ttu-id="a79ab-125">Общий вес всех качеств должен составлять не более 100.</span><span class="sxs-lookup"><span data-stu-id="a79ab-125">If present, weights must add up to 100.</span></span>

| | <span data-ttu-id="a79ab-126">Хорошо (2 балла)</span><span class="sxs-lookup"><span data-stu-id="a79ab-126">Good (2 points)</span></span> | <span data-ttu-id="a79ab-127">Плохо (1 балл)</span><span class="sxs-lookup"><span data-stu-id="a79ab-127">Poor (1 point)</span></span> |
|:--|:--|:--|
| <span data-ttu-id="a79ab-128">Аргументация (вес 50)</span><span class="sxs-lookup"><span data-stu-id="a79ab-128">Argument (weight 50)</span></span> | <span data-ttu-id="a79ab-129">Аргументы в сочинении убедительные.</span><span class="sxs-lookup"><span data-stu-id="a79ab-129">The essay's argument is persuasive.</span></span> | <span data-ttu-id="a79ab-130">Аргументы в сочинении не имеют смысла.</span><span class="sxs-lookup"><span data-stu-id="a79ab-130">The essay's argument does not make sense.</span></span> |
| <span data-ttu-id="a79ab-131">Правописание и грамматика (вес 50)</span><span class="sxs-lookup"><span data-stu-id="a79ab-131">Spelling and Grammar (weight 50)</span></span> | <span data-ttu-id="a79ab-132">В сочинении соблюдены орфографические и грамматические нормы. Ошибок немного или вообще нет.</span><span class="sxs-lookup"><span data-stu-id="a79ab-132">The essay uses proper spelling and grammar with few or no errors.</span></span> | <span data-ttu-id="a79ab-133">В сочинении много орфографических и грамматических ошибок.</span><span class="sxs-lookup"><span data-stu-id="a79ab-133">The essay has numerous errors in spelling and/or grammar.</span></span> |

## <a name="api-reference"></a><span data-ttu-id="a79ab-134">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="a79ab-134">API reference</span></span>

<span data-ttu-id="a79ab-135">Чтобы приступить к работе с рубриками, начните с[ресурса educationRubric в бета-версии Microsoft Graph](/graph/api/resources/educationrubric?view=graph-rest-beta) и связанных с ним методов.</span><span class="sxs-lookup"><span data-stu-id="a79ab-135">To begin using rubrics, start with the [educationRubric resource in Microsoft Graph beta](/graph/api/resources/educationrubric?view=graph-rest-beta) and associated methods.</span></span>





 

