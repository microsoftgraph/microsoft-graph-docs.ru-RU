---
title: Тип перечисления sharedPCAccountDeletionPolicyType
description: Возможные значения для при удалении учетных записей на общую ПК.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6a1e3c9e15409e253852b4b896e18181ef1bc391
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884128"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="c1c39-103">Тип перечисления sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="c1c39-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="c1c39-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1c39-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1c39-105">Возможные значения для при удалении учетных записей на общую ПК.</span><span class="sxs-lookup"><span data-stu-id="c1c39-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="c1c39-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c1c39-106">Members</span></span>
|<span data-ttu-id="c1c39-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c1c39-107">Member</span></span>|<span data-ttu-id="c1c39-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c1c39-108">Value</span></span>|<span data-ttu-id="c1c39-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c39-110">Интерпретация</span><span class="sxs-lookup"><span data-stu-id="c1c39-110">immediate</span></span>|<span data-ttu-id="c1c39-111">0</span><span class="sxs-lookup"><span data-stu-id="c1c39-111">0</span></span>|<span data-ttu-id="c1c39-112">Удаление немедленно.</span><span class="sxs-lookup"><span data-stu-id="c1c39-112">Delete immediately.</span></span>|
|<span data-ttu-id="c1c39-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="c1c39-113">diskSpaceThreshold</span></span>|<span data-ttu-id="c1c39-114">1</span><span class="sxs-lookup"><span data-stu-id="c1c39-114">1</span></span>|<span data-ttu-id="c1c39-115">Удалите в порога места на диске.</span><span class="sxs-lookup"><span data-stu-id="c1c39-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="c1c39-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="c1c39-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="c1c39-117">2</span><span class="sxs-lookup"><span data-stu-id="c1c39-117">2</span></span>|<span data-ttu-id="c1c39-118">Удалите порога места на диске, так и неактивных пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="c1c39-118">Delete at disk space threshold or inactive threshold.</span></span>|



