---
title: тип перечисления Виндовсдефендераппликатионконтролсупплементалполицистатусес
description: Перечисление значений различных состояний развертывания дополнительной политики Виндовсдефендераппликатионконтрол.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 851bb0a5544a807b1ae73cac15dfa5f788271703
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764098"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="cec6d-103">тип перечисления Виндовсдефендераппликатионконтролсупплементалполицистатусес</span><span class="sxs-lookup"><span data-stu-id="cec6d-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

> <span data-ttu-id="cec6d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec6d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cec6d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cec6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec6d-106">Перечисление значений различных состояний развертывания дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="cec6d-106">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="cec6d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="cec6d-107">Members</span></span>
|<span data-ttu-id="cec6d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="cec6d-108">Member</span></span>|<span data-ttu-id="cec6d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="cec6d-109">Value</span></span>|<span data-ttu-id="cec6d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cec6d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec6d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="cec6d-111">unknown</span></span>|<span data-ttu-id="cec6d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="cec6d-112">0</span></span>|<span data-ttu-id="cec6d-113">Состояние дополнительной политики Виндовсдефендераппликатионконтрол неизвестно.</span><span class="sxs-lookup"><span data-stu-id="cec6d-113">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="cec6d-114">success</span><span class="sxs-lookup"><span data-stu-id="cec6d-114">success</span></span>|<span data-ttu-id="cec6d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="cec6d-115">1</span></span>|<span data-ttu-id="cec6d-116">Применяется дополнительная политика Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="cec6d-116">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="cec6d-117">токенеррор</span><span class="sxs-lookup"><span data-stu-id="cec6d-117">tokenError</span></span>|<span data-ttu-id="cec6d-118">2</span><span class="sxs-lookup"><span data-stu-id="cec6d-118">2</span></span>|<span data-ttu-id="cec6d-119">Дополнительная политика Виндовсдефендераппликатионконтрол имеет структуру, но существует ошибка, связанная с авторизацией маркера.</span><span class="sxs-lookup"><span data-stu-id="cec6d-119">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="cec6d-120">нотаусоризедбитокен</span><span class="sxs-lookup"><span data-stu-id="cec6d-120">notAuthorizedByToken</span></span>|<span data-ttu-id="cec6d-121">4</span><span class="sxs-lookup"><span data-stu-id="cec6d-121">3</span></span>|<span data-ttu-id="cec6d-122">Маркер не авторизует эту дополнительную политику Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="cec6d-122">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="cec6d-123">полицинотфаунд</span><span class="sxs-lookup"><span data-stu-id="cec6d-123">policyNotFound</span></span>|<span data-ttu-id="cec6d-124">4 </span><span class="sxs-lookup"><span data-stu-id="cec6d-124">4</span></span>|<span data-ttu-id="cec6d-125">Дополнительная политика Виндовсдефендераппликатионконтрол не найдена.</span><span class="sxs-lookup"><span data-stu-id="cec6d-125">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



