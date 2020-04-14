---
title: тип перечисления Шаредпкаккаунтделетионполицитипе
description: Возможные значения для удаления учетных записей на общем компьютере.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 539591836b9771b1b00288c33f08c3db754f322d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443352"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="216cf-103">тип перечисления Шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="216cf-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="216cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="216cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="216cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="216cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="216cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="216cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="216cf-107">Возможные значения для удаления учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="216cf-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="216cf-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="216cf-108">Members</span></span>
|<span data-ttu-id="216cf-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="216cf-109">Member</span></span>|<span data-ttu-id="216cf-110">Значение</span><span class="sxs-lookup"><span data-stu-id="216cf-110">Value</span></span>|<span data-ttu-id="216cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="216cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="216cf-112">операнд</span><span class="sxs-lookup"><span data-stu-id="216cf-112">immediate</span></span>|<span data-ttu-id="216cf-113">нуль</span><span class="sxs-lookup"><span data-stu-id="216cf-113">0</span></span>|<span data-ttu-id="216cf-114">Немедленное удаление.</span><span class="sxs-lookup"><span data-stu-id="216cf-114">Delete immediately.</span></span>|
|<span data-ttu-id="216cf-115">дискспацесрешолд</span><span class="sxs-lookup"><span data-stu-id="216cf-115">diskSpaceThreshold</span></span>|<span data-ttu-id="216cf-116">1,1</span><span class="sxs-lookup"><span data-stu-id="216cf-116">1</span></span>|<span data-ttu-id="216cf-117">Удалить с порогового места на диске.</span><span class="sxs-lookup"><span data-stu-id="216cf-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="216cf-118">дискспацесрешолдоринактивесрешолд</span><span class="sxs-lookup"><span data-stu-id="216cf-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="216cf-119">2</span><span class="sxs-lookup"><span data-stu-id="216cf-119">2</span></span>|<span data-ttu-id="216cf-120">Удаление при пороговом значении или неактивном пороге места на диске.</span><span class="sxs-lookup"><span data-stu-id="216cf-120">Delete at disk space threshold or inactive threshold.</span></span>|



