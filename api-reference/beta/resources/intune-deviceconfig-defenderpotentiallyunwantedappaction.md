---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально неЖелательном приложении (ПУА).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1949ec58c7cfd2d896308f740b7eca16f2646b3e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800191"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="27462-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="27462-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="27462-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27462-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27462-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27462-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27462-106">Действие защитника, которое будет принимать участие в обнаруженном потенциально неЖелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="27462-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="27462-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="27462-107">Members</span></span>
|<span data-ttu-id="27462-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="27462-108">Member</span></span>|<span data-ttu-id="27462-109">Значение</span><span class="sxs-lookup"><span data-stu-id="27462-109">Value</span></span>|<span data-ttu-id="27462-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27462-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27462-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="27462-111">deviceDefault</span></span>|<span data-ttu-id="27462-112">нуль</span><span class="sxs-lookup"><span data-stu-id="27462-112">0</span></span>|<span data-ttu-id="27462-113">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="27462-113">PUA Protection is off.</span></span> <span data-ttu-id="27462-114">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="27462-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="27462-115">блок</span><span class="sxs-lookup"><span data-stu-id="27462-115">block</span></span>|<span data-ttu-id="27462-116">1,1</span><span class="sxs-lookup"><span data-stu-id="27462-116">1</span></span>|<span data-ttu-id="27462-117">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="27462-117">PUA Protection is on.</span></span> <span data-ttu-id="27462-118">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="27462-118">Detected items are blocked.</span></span> <span data-ttu-id="27462-119">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="27462-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="27462-120">включить</span><span class="sxs-lookup"><span data-stu-id="27462-120">audit</span></span>|<span data-ttu-id="27462-121">2</span><span class="sxs-lookup"><span data-stu-id="27462-121">2</span></span>|<span data-ttu-id="27462-122">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="27462-122">Audit mode.</span></span> <span data-ttu-id="27462-123">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="27462-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="27462-124">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="27462-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





