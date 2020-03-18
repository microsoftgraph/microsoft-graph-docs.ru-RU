---
title: тип перечисления Полицисетстатус
description: Перечисление, указывающее состояние набора политик.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a470e6c13bfd20ada920bbe2b471bfa96379092
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775151"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="b1068-103">тип перечисления Полицисетстатус</span><span class="sxs-lookup"><span data-stu-id="b1068-103">policySetStatus enum type</span></span>

> <span data-ttu-id="b1068-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1068-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1068-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1068-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1068-106">Перечисление, указывающее состояние набора политик.</span><span class="sxs-lookup"><span data-stu-id="b1068-106">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="b1068-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b1068-107">Members</span></span>
|<span data-ttu-id="b1068-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b1068-108">Member</span></span>|<span data-ttu-id="b1068-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b1068-109">Value</span></span>|<span data-ttu-id="b1068-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1068-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1068-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b1068-111">unknown</span></span>|<span data-ttu-id="b1068-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b1068-112">0</span></span>|<span data-ttu-id="b1068-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b1068-113">Default Value.</span></span>|
|<span data-ttu-id="b1068-114">нарушение</span><span class="sxs-lookup"><span data-stu-id="b1068-114">validating</span></span>|<span data-ttu-id="b1068-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b1068-115">1</span></span>|<span data-ttu-id="b1068-116">Все элементы набора политик теперь проверяют соответствующие параметры рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="b1068-116">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="b1068-117">партиалсукцесс</span><span class="sxs-lookup"><span data-stu-id="b1068-117">partialSuccess</span></span>|<span data-ttu-id="b1068-118">2</span><span class="sxs-lookup"><span data-stu-id="b1068-118">2</span></span>|<span data-ttu-id="b1068-119">POST завершен для всех элементов с политиками, но существуют ошибки.</span><span class="sxs-lookup"><span data-stu-id="b1068-119">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="b1068-120">success</span><span class="sxs-lookup"><span data-stu-id="b1068-120">success</span></span>|<span data-ttu-id="b1068-121">4</span><span class="sxs-lookup"><span data-stu-id="b1068-121">3</span></span>|<span data-ttu-id="b1068-122">Все элементы с развернутыми политиками.</span><span class="sxs-lookup"><span data-stu-id="b1068-122">All PolicySet items are deployed.</span></span> <span data-ttu-id="b1068-123">Не означает, что развертывание завершено успешно.</span><span class="sxs-lookup"><span data-stu-id="b1068-123">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="b1068-124">error</span><span class="sxs-lookup"><span data-stu-id="b1068-124">error</span></span>|<span data-ttu-id="b1068-125">4 </span><span class="sxs-lookup"><span data-stu-id="b1068-125">4</span></span>|<span data-ttu-id="b1068-126">Обработка подполитики завершена с ошибками.</span><span class="sxs-lookup"><span data-stu-id="b1068-126">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="b1068-127">нотассигнед</span><span class="sxs-lookup"><span data-stu-id="b1068-127">notAssigned</span></span>|<span data-ttu-id="b1068-128">5 </span><span class="sxs-lookup"><span data-stu-id="b1068-128">5</span></span>|<span data-ttu-id="b1068-129">Policy/Полицисетитем не назначено ни одной группе.</span><span class="sxs-lookup"><span data-stu-id="b1068-129">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



