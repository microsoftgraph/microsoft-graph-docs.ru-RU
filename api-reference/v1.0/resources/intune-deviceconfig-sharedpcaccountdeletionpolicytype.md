---
title: тип enum sharedPCAccountDeletionPolicyType
description: Возможные значения при удалении учетных записей на общем компьютере.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a3b4245ccf1a5a03d8b2142b65bfed69685de254
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751722"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="10864-103">тип enum sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="10864-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="10864-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10864-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10864-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10864-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10864-106">Возможные значения при удалении учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="10864-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="10864-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="10864-107">Members</span></span>
|<span data-ttu-id="10864-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="10864-108">Member</span></span>|<span data-ttu-id="10864-109">Значение</span><span class="sxs-lookup"><span data-stu-id="10864-109">Value</span></span>|<span data-ttu-id="10864-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10864-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10864-111">немедленная</span><span class="sxs-lookup"><span data-stu-id="10864-111">immediate</span></span>|<span data-ttu-id="10864-112">0</span><span class="sxs-lookup"><span data-stu-id="10864-112">0</span></span>|<span data-ttu-id="10864-113">Удалите немедленно.</span><span class="sxs-lookup"><span data-stu-id="10864-113">Delete immediately.</span></span>|
|<span data-ttu-id="10864-114">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="10864-114">diskSpaceThreshold</span></span>|<span data-ttu-id="10864-115">1</span><span class="sxs-lookup"><span data-stu-id="10864-115">1</span></span>|<span data-ttu-id="10864-116">Удаление на пороге пространства диска.</span><span class="sxs-lookup"><span data-stu-id="10864-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="10864-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="10864-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="10864-118">2</span><span class="sxs-lookup"><span data-stu-id="10864-118">2</span></span>|<span data-ttu-id="10864-119">Удаление на дисковом пороге пространства или неактивном пороге.</span><span class="sxs-lookup"><span data-stu-id="10864-119">Delete at disk space threshold or inactive threshold.</span></span>|




