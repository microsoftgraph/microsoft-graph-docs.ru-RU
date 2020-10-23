---
title: тип перечисления Шаредпкаккаунтделетионполицитипе
description: Возможные значения для удаления учетных записей на общем компьютере.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d40e845333a5702813fb00b4c678f67648aeadca
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709877"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="89a93-103">тип перечисления Шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="89a93-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="89a93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89a93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89a93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89a93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89a93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89a93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89a93-107">Возможные значения для удаления учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="89a93-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="89a93-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="89a93-108">Members</span></span>
|<span data-ttu-id="89a93-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="89a93-109">Member</span></span>|<span data-ttu-id="89a93-110">Значение</span><span class="sxs-lookup"><span data-stu-id="89a93-110">Value</span></span>|<span data-ttu-id="89a93-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89a93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89a93-112">операнд</span><span class="sxs-lookup"><span data-stu-id="89a93-112">immediate</span></span>|<span data-ttu-id="89a93-113">нуль</span><span class="sxs-lookup"><span data-stu-id="89a93-113">0</span></span>|<span data-ttu-id="89a93-114">Немедленное удаление.</span><span class="sxs-lookup"><span data-stu-id="89a93-114">Delete immediately.</span></span>|
|<span data-ttu-id="89a93-115">дискспацесрешолд</span><span class="sxs-lookup"><span data-stu-id="89a93-115">diskSpaceThreshold</span></span>|<span data-ttu-id="89a93-116">1,1</span><span class="sxs-lookup"><span data-stu-id="89a93-116">1</span></span>|<span data-ttu-id="89a93-117">Удалить с порогового места на диске.</span><span class="sxs-lookup"><span data-stu-id="89a93-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="89a93-118">дискспацесрешолдоринактивесрешолд</span><span class="sxs-lookup"><span data-stu-id="89a93-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="89a93-119">2</span><span class="sxs-lookup"><span data-stu-id="89a93-119">2</span></span>|<span data-ttu-id="89a93-120">Удаление при пороговом значении или неактивном пороге места на диске.</span><span class="sxs-lookup"><span data-stu-id="89a93-120">Delete at disk space threshold or inactive threshold.</span></span>|





