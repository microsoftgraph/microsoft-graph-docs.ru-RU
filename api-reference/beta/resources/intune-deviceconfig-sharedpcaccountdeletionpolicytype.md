---
title: тип перечисления Шаредпкаккаунтделетионполицитипе
description: Возможные значения для удаления учетных записей на общем компьютере.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a0f86e9d3fac7fcc53e5f593078b2d073d4e353
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293740"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="f11fb-103">тип перечисления Шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="f11fb-103">sharedPCAccountDeletionPolicyType enum type</span></span>

<span data-ttu-id="f11fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f11fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f11fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f11fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f11fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f11fb-107">Возможные значения для удаления учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="f11fb-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="f11fb-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f11fb-108">Members</span></span>
|<span data-ttu-id="f11fb-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f11fb-109">Member</span></span>|<span data-ttu-id="f11fb-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f11fb-110">Value</span></span>|<span data-ttu-id="f11fb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f11fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11fb-112">операнд</span><span class="sxs-lookup"><span data-stu-id="f11fb-112">immediate</span></span>|<span data-ttu-id="f11fb-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f11fb-113">0</span></span>|<span data-ttu-id="f11fb-114">Немедленное удаление.</span><span class="sxs-lookup"><span data-stu-id="f11fb-114">Delete immediately.</span></span>|
|<span data-ttu-id="f11fb-115">дискспацесрешолд</span><span class="sxs-lookup"><span data-stu-id="f11fb-115">diskSpaceThreshold</span></span>|<span data-ttu-id="f11fb-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f11fb-116">1</span></span>|<span data-ttu-id="f11fb-117">Удалить с порогового места на диске.</span><span class="sxs-lookup"><span data-stu-id="f11fb-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="f11fb-118">дискспацесрешолдоринактивесрешолд</span><span class="sxs-lookup"><span data-stu-id="f11fb-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="f11fb-119">2</span><span class="sxs-lookup"><span data-stu-id="f11fb-119">2</span></span>|<span data-ttu-id="f11fb-120">Удаление при пороговом значении или неактивном пороге места на диске.</span><span class="sxs-lookup"><span data-stu-id="f11fb-120">Delete at disk space threshold or inactive threshold.</span></span>|




