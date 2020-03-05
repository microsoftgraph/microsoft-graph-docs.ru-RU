---
title: тип перечисления Шаредпкаккаунтделетионполицитипе
description: Возможные значения для удаления учетных записей на общем компьютере.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f843aaf9ace8f41aa83b34993a2229cac91877f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525868"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="ebb99-103">тип перечисления Шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="ebb99-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="ebb99-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ebb99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebb99-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebb99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebb99-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebb99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb99-107">Возможные значения для удаления учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="ebb99-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="ebb99-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ebb99-108">Members</span></span>
|<span data-ttu-id="ebb99-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ebb99-109">Member</span></span>|<span data-ttu-id="ebb99-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ebb99-110">Value</span></span>|<span data-ttu-id="ebb99-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb99-112">операнд</span><span class="sxs-lookup"><span data-stu-id="ebb99-112">immediate</span></span>|<span data-ttu-id="ebb99-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ebb99-113">0</span></span>|<span data-ttu-id="ebb99-114">Немедленное удаление.</span><span class="sxs-lookup"><span data-stu-id="ebb99-114">Delete immediately.</span></span>|
|<span data-ttu-id="ebb99-115">дискспацесрешолд</span><span class="sxs-lookup"><span data-stu-id="ebb99-115">diskSpaceThreshold</span></span>|<span data-ttu-id="ebb99-116">1 </span><span class="sxs-lookup"><span data-stu-id="ebb99-116">1</span></span>|<span data-ttu-id="ebb99-117">Удалить с порогового места на диске.</span><span class="sxs-lookup"><span data-stu-id="ebb99-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="ebb99-118">дискспацесрешолдоринактивесрешолд</span><span class="sxs-lookup"><span data-stu-id="ebb99-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="ebb99-119">2 </span><span class="sxs-lookup"><span data-stu-id="ebb99-119">2</span></span>|<span data-ttu-id="ebb99-120">Удаление при пороговом значении или неактивном пороге места на диске.</span><span class="sxs-lookup"><span data-stu-id="ebb99-120">Delete at disk space threshold or inactive threshold.</span></span>|



