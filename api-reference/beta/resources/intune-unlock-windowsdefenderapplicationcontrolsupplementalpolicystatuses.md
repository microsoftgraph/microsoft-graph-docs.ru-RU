---
title: тип перечисления Виндовсдефендераппликатионконтролсупплементалполицистатусес
description: Перечисление значений различных состояний развертывания дополнительной политики Виндовсдефендераппликатионконтрол.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1999c999597d152396590e3faee6d7b472189500
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537659"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="f0fa6-103">тип перечисления Виндовсдефендераппликатионконтролсупплементалполицистатусес</span><span class="sxs-lookup"><span data-stu-id="f0fa6-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

> <span data-ttu-id="f0fa6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0fa6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0fa6-106">Перечисление значений различных состояний развертывания дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-106">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="f0fa6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f0fa6-107">Members</span></span>
|<span data-ttu-id="f0fa6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f0fa6-108">Member</span></span>|<span data-ttu-id="f0fa6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f0fa6-109">Value</span></span>|<span data-ttu-id="f0fa6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0fa6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0fa6-111">unknown</span><span class="sxs-lookup"><span data-stu-id="f0fa6-111">unknown</span></span>|<span data-ttu-id="f0fa6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f0fa6-112">0</span></span>|<span data-ttu-id="f0fa6-113">Состояние дополнительной политики Виндовсдефендераппликатионконтрол неизвестно.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-113">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="f0fa6-114">success</span><span class="sxs-lookup"><span data-stu-id="f0fa6-114">success</span></span>|<span data-ttu-id="f0fa6-115">1,1</span><span class="sxs-lookup"><span data-stu-id="f0fa6-115">1</span></span>|<span data-ttu-id="f0fa6-116">Применяется дополнительная политика Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-116">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="f0fa6-117">токенеррор</span><span class="sxs-lookup"><span data-stu-id="f0fa6-117">tokenError</span></span>|<span data-ttu-id="f0fa6-118">2</span><span class="sxs-lookup"><span data-stu-id="f0fa6-118">2</span></span>|<span data-ttu-id="f0fa6-119">Дополнительная политика Виндовсдефендераппликатионконтрол имеет структуру, но существует ошибка, связанная с авторизацией маркера.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-119">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="f0fa6-120">нотаусоризедбитокен</span><span class="sxs-lookup"><span data-stu-id="f0fa6-120">notAuthorizedByToken</span></span>|<span data-ttu-id="f0fa6-121">4</span><span class="sxs-lookup"><span data-stu-id="f0fa6-121">3</span></span>|<span data-ttu-id="f0fa6-122">Маркер не авторизует эту дополнительную политику Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-122">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="f0fa6-123">полицинотфаунд</span><span class="sxs-lookup"><span data-stu-id="f0fa6-123">policyNotFound</span></span>|<span data-ttu-id="f0fa6-124">4 </span><span class="sxs-lookup"><span data-stu-id="f0fa6-124">4</span></span>|<span data-ttu-id="f0fa6-125">Дополнительная политика Виндовсдефендераппликатионконтрол не найдена.</span><span class="sxs-lookup"><span data-stu-id="f0fa6-125">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



