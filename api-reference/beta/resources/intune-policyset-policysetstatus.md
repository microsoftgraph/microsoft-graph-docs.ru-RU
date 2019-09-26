---
title: тип перечисления Полицисетстатус
description: Перечисление, указывающее состояние набора политик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a41e4f3dc01bd04c915dc4c883bae640b3e7683
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201251"
---
# <a name="policysetstatus-enum-type"></a><span data-ttu-id="66a54-103">тип перечисления Полицисетстатус</span><span class="sxs-lookup"><span data-stu-id="66a54-103">policySetStatus enum type</span></span>

> <span data-ttu-id="66a54-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66a54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66a54-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66a54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66a54-106">Перечисление, указывающее состояние набора политик.</span><span class="sxs-lookup"><span data-stu-id="66a54-106">The enum to specify the status of PolicySet.</span></span>

## <a name="members"></a><span data-ttu-id="66a54-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="66a54-107">Members</span></span>
|<span data-ttu-id="66a54-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="66a54-108">Member</span></span>|<span data-ttu-id="66a54-109">Значение</span><span class="sxs-lookup"><span data-stu-id="66a54-109">Value</span></span>|<span data-ttu-id="66a54-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66a54-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66a54-111">unknown</span><span class="sxs-lookup"><span data-stu-id="66a54-111">unknown</span></span>|<span data-ttu-id="66a54-112">нуль</span><span class="sxs-lookup"><span data-stu-id="66a54-112">0</span></span>|<span data-ttu-id="66a54-113">Значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="66a54-113">Default Value.</span></span>|
|<span data-ttu-id="66a54-114">нарушение</span><span class="sxs-lookup"><span data-stu-id="66a54-114">validating</span></span>|<span data-ttu-id="66a54-115">1,1</span><span class="sxs-lookup"><span data-stu-id="66a54-115">1</span></span>|<span data-ttu-id="66a54-116">Все элементы набора политик теперь проверяют соответствующие параметры рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="66a54-116">All PolicySet items are now validating for corresponding settings of workloads.</span></span>|
|<span data-ttu-id="66a54-117">партиалсукцесс</span><span class="sxs-lookup"><span data-stu-id="66a54-117">partialSuccess</span></span>|<span data-ttu-id="66a54-118">2</span><span class="sxs-lookup"><span data-stu-id="66a54-118">2</span></span>|<span data-ttu-id="66a54-119">POST завершен для всех элементов с политиками, но существуют ошибки.</span><span class="sxs-lookup"><span data-stu-id="66a54-119">Post process complete for all PolicySet items but there are failures.</span></span>|
|<span data-ttu-id="66a54-120">success</span><span class="sxs-lookup"><span data-stu-id="66a54-120">success</span></span>|<span data-ttu-id="66a54-121">4</span><span class="sxs-lookup"><span data-stu-id="66a54-121">3</span></span>|<span data-ttu-id="66a54-122">Все элементы с развернутыми политиками.</span><span class="sxs-lookup"><span data-stu-id="66a54-122">All PolicySet items are deployed.</span></span> <span data-ttu-id="66a54-123">Не означает, что развертывание завершено успешно.</span><span class="sxs-lookup"><span data-stu-id="66a54-123">Doesn’t mean that all deployment succeeded.</span></span> |
|<span data-ttu-id="66a54-124">error</span><span class="sxs-lookup"><span data-stu-id="66a54-124">error</span></span>|<span data-ttu-id="66a54-125">SP4</span><span class="sxs-lookup"><span data-stu-id="66a54-125">4</span></span>|<span data-ttu-id="66a54-126">Обработка подполитики завершена с ошибками.</span><span class="sxs-lookup"><span data-stu-id="66a54-126">PolicySet processing completely failed.</span></span>|
|<span data-ttu-id="66a54-127">нотассигнед</span><span class="sxs-lookup"><span data-stu-id="66a54-127">notAssigned</span></span>|<span data-ttu-id="66a54-128">17:00</span><span class="sxs-lookup"><span data-stu-id="66a54-128">5</span></span>|<span data-ttu-id="66a54-129">Policy/Полицисетитем не назначено ни одной группе.</span><span class="sxs-lookup"><span data-stu-id="66a54-129">PolicySet/PolicySetItem is not assigned to any group.</span></span>|



