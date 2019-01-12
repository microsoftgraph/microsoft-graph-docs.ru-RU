---
title: Тип перечисления sharedPCAccountDeletionPolicyType
description: Возможные значения для при удалении учетных записей на общую ПК.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5dc216d20becdc233bd1664250a958aa7208f1c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937630"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="beb75-103">Тип перечисления sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="beb75-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="beb75-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="beb75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beb75-105">Возможные значения для при удалении учетных записей на общую ПК.</span><span class="sxs-lookup"><span data-stu-id="beb75-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="beb75-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="beb75-106">Members</span></span>
|<span data-ttu-id="beb75-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="beb75-107">Member</span></span>|<span data-ttu-id="beb75-108">Значение</span><span class="sxs-lookup"><span data-stu-id="beb75-108">Value</span></span>|<span data-ttu-id="beb75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="beb75-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb75-110">Интерпретация</span><span class="sxs-lookup"><span data-stu-id="beb75-110">immediate</span></span>|<span data-ttu-id="beb75-111">0</span><span class="sxs-lookup"><span data-stu-id="beb75-111">0</span></span>|<span data-ttu-id="beb75-112">Удаление немедленно.</span><span class="sxs-lookup"><span data-stu-id="beb75-112">Delete immediately.</span></span>|
|<span data-ttu-id="beb75-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="beb75-113">diskSpaceThreshold</span></span>|<span data-ttu-id="beb75-114">1</span><span class="sxs-lookup"><span data-stu-id="beb75-114">1</span></span>|<span data-ttu-id="beb75-115">Удалите в порога места на диске.</span><span class="sxs-lookup"><span data-stu-id="beb75-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="beb75-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="beb75-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="beb75-117">2</span><span class="sxs-lookup"><span data-stu-id="beb75-117">2</span></span>|<span data-ttu-id="beb75-118">Удалите порога места на диске, так и неактивных пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="beb75-118">Delete at disk space threshold or inactive threshold.</span></span>|



