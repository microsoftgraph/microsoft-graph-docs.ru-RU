---
title: тип перечисления Полицисетстатус
description: Перечисление, указывающее состояние набора политик.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 32ea9586ffee2ef112c58a1f88bdbdaefd654a04
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735164"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="a48a1-103">тип перечисления Полицисетстатус</span><span class="sxs-lookup"><span data-stu-id="a48a1-103">policySetStatus enum type</span></span>

<span data-ttu-id="a48a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a48a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a48a1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a48a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a48a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a48a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a48a1-107">Перечисление, указывающее состояние набора политик.</span><span class="sxs-lookup"><span data-stu-id="a48a1-107">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="a48a1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a48a1-108">Members</span></span>
|<span data-ttu-id="a48a1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a48a1-109">Member</span></span>|<span data-ttu-id="a48a1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a48a1-110">Value</span></span>|<span data-ttu-id="a48a1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a48a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a48a1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="a48a1-112">unknown</span></span>|<span data-ttu-id="a48a1-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a48a1-113">0</span></span>|<span data-ttu-id="a48a1-114">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a48a1-114">Default Value.</span></span>|
|<span data-ttu-id="a48a1-115">нарушение</span><span class="sxs-lookup"><span data-stu-id="a48a1-115">validating</span></span>|<span data-ttu-id="a48a1-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a48a1-116">1</span></span>|<span data-ttu-id="a48a1-117">Все элементы набора политик теперь проверяют соответствующие параметры рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="a48a1-117">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="a48a1-118">партиалсукцесс</span><span class="sxs-lookup"><span data-stu-id="a48a1-118">partialSuccess</span></span>|<span data-ttu-id="a48a1-119">2</span><span class="sxs-lookup"><span data-stu-id="a48a1-119">2</span></span>|<span data-ttu-id="a48a1-120">POST завершен для всех элементов с политиками, но существуют ошибки.</span><span class="sxs-lookup"><span data-stu-id="a48a1-120">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="a48a1-121">success</span><span class="sxs-lookup"><span data-stu-id="a48a1-121">success</span></span>|<span data-ttu-id="a48a1-122">4</span><span class="sxs-lookup"><span data-stu-id="a48a1-122">3</span></span>|<span data-ttu-id="a48a1-123">Все элементы с развернутыми политиками.</span><span class="sxs-lookup"><span data-stu-id="a48a1-123">All PolicySet items are deployed.</span></span> <span data-ttu-id="a48a1-124">Не означает, что развертывание завершено успешно.</span><span class="sxs-lookup"><span data-stu-id="a48a1-124">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="a48a1-125">error</span><span class="sxs-lookup"><span data-stu-id="a48a1-125">error</span></span>|<span data-ttu-id="a48a1-126">4 </span><span class="sxs-lookup"><span data-stu-id="a48a1-126">4</span></span>|<span data-ttu-id="a48a1-127">Обработка подполитики завершена с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a48a1-127">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="a48a1-128">нотассигнед</span><span class="sxs-lookup"><span data-stu-id="a48a1-128">notAssigned</span></span>|<span data-ttu-id="a48a1-129">5 </span><span class="sxs-lookup"><span data-stu-id="a48a1-129">5</span></span>|<span data-ttu-id="a48a1-130">Policy/Полицисетитем не назначено ни одной группе.</span><span class="sxs-lookup"><span data-stu-id="a48a1-130">PolicySet/PolicySetItem is not assigned to any group.</span></span>|





