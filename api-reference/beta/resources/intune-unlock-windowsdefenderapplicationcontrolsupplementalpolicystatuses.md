---
title: тип перечисления Виндовсдефендераппликатионконтролсупплементалполицистатусес
description: Перечисление значений различных состояний развертывания дополнительной политики Виндовсдефендераппликатионконтрол.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a8d1ecab8f108cbf885421a760671b13075ed87b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265942"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="16a9f-103">тип перечисления Виндовсдефендераппликатионконтролсупплементалполицистатусес</span><span class="sxs-lookup"><span data-stu-id="16a9f-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

<span data-ttu-id="16a9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16a9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16a9f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16a9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16a9f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16a9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16a9f-107">Перечисление значений различных состояний развертывания дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="16a9f-107">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="16a9f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="16a9f-108">Members</span></span>
|<span data-ttu-id="16a9f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="16a9f-109">Member</span></span>|<span data-ttu-id="16a9f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="16a9f-110">Value</span></span>|<span data-ttu-id="16a9f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16a9f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16a9f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="16a9f-112">unknown</span></span>|<span data-ttu-id="16a9f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="16a9f-113">0</span></span>|<span data-ttu-id="16a9f-114">Состояние дополнительной политики Виндовсдефендераппликатионконтрол неизвестно.</span><span class="sxs-lookup"><span data-stu-id="16a9f-114">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="16a9f-115">success</span><span class="sxs-lookup"><span data-stu-id="16a9f-115">success</span></span>|<span data-ttu-id="16a9f-116">1,1</span><span class="sxs-lookup"><span data-stu-id="16a9f-116">1</span></span>|<span data-ttu-id="16a9f-117">Применяется дополнительная политика Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="16a9f-117">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="16a9f-118">токенеррор</span><span class="sxs-lookup"><span data-stu-id="16a9f-118">tokenError</span></span>|<span data-ttu-id="16a9f-119">2</span><span class="sxs-lookup"><span data-stu-id="16a9f-119">2</span></span>|<span data-ttu-id="16a9f-120">Дополнительная политика Виндовсдефендераппликатионконтрол имеет структуру, но существует ошибка, связанная с авторизацией маркера.</span><span class="sxs-lookup"><span data-stu-id="16a9f-120">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="16a9f-121">нотаусоризедбитокен</span><span class="sxs-lookup"><span data-stu-id="16a9f-121">notAuthorizedByToken</span></span>|<span data-ttu-id="16a9f-122">4</span><span class="sxs-lookup"><span data-stu-id="16a9f-122">3</span></span>|<span data-ttu-id="16a9f-123">Маркер не авторизует эту дополнительную политику Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="16a9f-123">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="16a9f-124">полицинотфаунд</span><span class="sxs-lookup"><span data-stu-id="16a9f-124">policyNotFound</span></span>|<span data-ttu-id="16a9f-125">4 </span><span class="sxs-lookup"><span data-stu-id="16a9f-125">4</span></span>|<span data-ttu-id="16a9f-126">Дополнительная политика Виндовсдефендераппликатионконтрол не найдена.</span><span class="sxs-lookup"><span data-stu-id="16a9f-126">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|




