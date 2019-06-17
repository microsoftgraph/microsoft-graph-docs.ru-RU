---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3816fe9e4366d21ddab43558ea6ab703a2d4d660
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979860"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="4a7d2-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="4a7d2-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="4a7d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a7d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a7d2-106">Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="4a7d2-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="4a7d2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4a7d2-107">Members</span></span>
|<span data-ttu-id="4a7d2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4a7d2-108">Member</span></span>|<span data-ttu-id="4a7d2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4a7d2-109">Value</span></span>|<span data-ttu-id="4a7d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4a7d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a7d2-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="4a7d2-111">deviceDefault</span></span>|<span data-ttu-id="4a7d2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4a7d2-112">0</span></span>|<span data-ttu-id="4a7d2-113">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-113">PUA Protection is off.</span></span> <span data-ttu-id="4a7d2-114">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="4a7d2-115">блок</span><span class="sxs-lookup"><span data-stu-id="4a7d2-115">block</span></span>|<span data-ttu-id="4a7d2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="4a7d2-116">1</span></span>|<span data-ttu-id="4a7d2-117">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-117">PUA Protection is on.</span></span> <span data-ttu-id="4a7d2-118">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-118">Detected items are blocked.</span></span> <span data-ttu-id="4a7d2-119">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="4a7d2-120">включить</span><span class="sxs-lookup"><span data-stu-id="4a7d2-120">audit</span></span>|<span data-ttu-id="4a7d2-121">2</span><span class="sxs-lookup"><span data-stu-id="4a7d2-121">2</span></span>|<span data-ttu-id="4a7d2-122">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-122">Audit mode.</span></span> <span data-ttu-id="4a7d2-123">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="4a7d2-124">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="4a7d2-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





