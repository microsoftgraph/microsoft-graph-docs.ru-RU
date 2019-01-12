---
title: Тип перечисления teamSpecialization
description: Описание варианта использования специальных для команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930287"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="375db-103">Тип перечисления teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="375db-103">teamSpecialization enum type</span></span>

> <span data-ttu-id="375db-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="375db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="375db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="375db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="375db-106">Указывает, будет ли [группы](../resources/team.md) для конкретного варианта использования.</span><span class="sxs-lookup"><span data-stu-id="375db-106">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="375db-107">Специализация каждой [группы](../resources/team.md) имеет доступ к уникальное поведение и каждый раз, нацелено на пример его использования.</span><span class="sxs-lookup"><span data-stu-id="375db-107">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="375db-108">Значение по умолчанию — «none».</span><span class="sxs-lookup"><span data-stu-id="375db-108">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="375db-109">Элементы</span><span class="sxs-lookup"><span data-stu-id="375db-109">Members</span></span>

| <span data-ttu-id="375db-110">Элемент</span><span class="sxs-lookup"><span data-stu-id="375db-110">Member</span></span>             | <span data-ttu-id="375db-111">Значение</span><span class="sxs-lookup"><span data-stu-id="375db-111">Value</span></span> | <span data-ttu-id="375db-112">Описание</span><span class="sxs-lookup"><span data-stu-id="375db-112">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="375db-113">Нет</span><span class="sxs-lookup"><span data-stu-id="375db-113">none</span></span>               | <span data-ttu-id="375db-114">0</span><span class="sxs-lookup"><span data-stu-id="375db-114">0</span></span>     | <span data-ttu-id="375db-115">Тип для группы, которая предоставляет опыт стандартной рабочей группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="375db-115">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="375db-116">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="375db-116">unknownFutureValue</span></span> | <span data-ttu-id="375db-117">7</span><span class="sxs-lookup"><span data-stu-id="375db-117">7</span></span>     | <span data-ttu-id="375db-118">Sentinel значение зарезервировано для выполнения будущее расширение перечисления.</span><span class="sxs-lookup"><span data-stu-id="375db-118">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
