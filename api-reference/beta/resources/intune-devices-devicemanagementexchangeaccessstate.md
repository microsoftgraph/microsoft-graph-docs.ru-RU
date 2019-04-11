---
title: тип перечисления Девицеманажементексчанжеакцессстате
description: Состояние доступа к Exchange для устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3cbe04dee84418d43dc610253522174caad9b2f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788494"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="5b444-103">тип перечисления Девицеманажементексчанжеакцессстате</span><span class="sxs-lookup"><span data-stu-id="5b444-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="5b444-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b444-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b444-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b444-106">Состояние доступа к Exchange для устройства.</span><span class="sxs-lookup"><span data-stu-id="5b444-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="5b444-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5b444-107">Members</span></span>
|<span data-ttu-id="5b444-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5b444-108">Member</span></span>|<span data-ttu-id="5b444-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5b444-109">Value</span></span>|<span data-ttu-id="5b444-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b444-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b444-111">нет</span><span class="sxs-lookup"><span data-stu-id="5b444-111">none</span></span>|<span data-ttu-id="5b444-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5b444-112">0</span></span>|<span data-ttu-id="5b444-113">Не обнаружено состояние доступа в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b444-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="5b444-114">unknown</span><span class="sxs-lookup"><span data-stu-id="5b444-114">unknown</span></span>|<span data-ttu-id="5b444-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5b444-115">1</span></span>|<span data-ttu-id="5b444-116">Неизвестный режим доступа к устройству Exchange</span><span class="sxs-lookup"><span data-stu-id="5b444-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="5b444-117">разрешенных</span><span class="sxs-lookup"><span data-stu-id="5b444-117">allowed</span></span>|<span data-ttu-id="5b444-118">2</span><span class="sxs-lookup"><span data-stu-id="5b444-118">2</span></span>|<span data-ttu-id="5b444-119">Устройство имеет доступ к Exchange</span><span class="sxs-lookup"><span data-stu-id="5b444-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="5b444-120">заблокированных</span><span class="sxs-lookup"><span data-stu-id="5b444-120">blocked</span></span>|<span data-ttu-id="5b444-121">4</span><span class="sxs-lookup"><span data-stu-id="5b444-121">3</span></span>|<span data-ttu-id="5b444-122">Устройство заблокировано в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b444-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="5b444-123">карантин</span><span class="sxs-lookup"><span data-stu-id="5b444-123">quarantined</span></span>|<span data-ttu-id="5b444-124">SP4</span><span class="sxs-lookup"><span data-stu-id="5b444-124">4</span></span>|<span data-ttu-id="5b444-125">Устройство помещено в карантин в Exchange</span><span class="sxs-lookup"><span data-stu-id="5b444-125">Device is Quarantined in Exchange</span></span>|





