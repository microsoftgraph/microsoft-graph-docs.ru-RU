---
title: тип перечисления Шаредпкаккаунтделетионполицитипе
description: Возможные значения для удаления учетных записей на общем компьютере.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 45c695e1fb55617516905e25e4667a15b8f66c6c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787546"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="8f636-103">тип перечисления Шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="8f636-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="8f636-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f636-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f636-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f636-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f636-106">Возможные значения для удаления учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="8f636-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="8f636-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8f636-107">Members</span></span>
|<span data-ttu-id="8f636-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8f636-108">Member</span></span>|<span data-ttu-id="8f636-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8f636-109">Value</span></span>|<span data-ttu-id="8f636-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f636-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f636-111">операнд</span><span class="sxs-lookup"><span data-stu-id="8f636-111">immediate</span></span>|<span data-ttu-id="8f636-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8f636-112">0</span></span>|<span data-ttu-id="8f636-113">Немедленное удаление.</span><span class="sxs-lookup"><span data-stu-id="8f636-113">Delete immediately.</span></span>|
|<span data-ttu-id="8f636-114">дискспацесрешолд</span><span class="sxs-lookup"><span data-stu-id="8f636-114">diskSpaceThreshold</span></span>|<span data-ttu-id="8f636-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8f636-115">1</span></span>|<span data-ttu-id="8f636-116">Удалить с порогового места на диске.</span><span class="sxs-lookup"><span data-stu-id="8f636-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="8f636-117">дискспацесрешолдоринактивесрешолд</span><span class="sxs-lookup"><span data-stu-id="8f636-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="8f636-118">2</span><span class="sxs-lookup"><span data-stu-id="8f636-118">2</span></span>|<span data-ttu-id="8f636-119">Удаление при пороговом значении или неактивном пороге места на диске.</span><span class="sxs-lookup"><span data-stu-id="8f636-119">Delete at disk space threshold or inactive threshold.</span></span>|



