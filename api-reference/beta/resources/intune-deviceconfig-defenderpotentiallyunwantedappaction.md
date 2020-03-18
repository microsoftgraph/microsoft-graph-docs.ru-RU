---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0c99cf04b217239fb1a06b2a6c26dcacc6c61cf7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794468"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="11304-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="11304-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="11304-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11304-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11304-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11304-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11304-106">Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="11304-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="11304-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="11304-107">Members</span></span>
|<span data-ttu-id="11304-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="11304-108">Member</span></span>|<span data-ttu-id="11304-109">Значение</span><span class="sxs-lookup"><span data-stu-id="11304-109">Value</span></span>|<span data-ttu-id="11304-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11304-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11304-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="11304-111">deviceDefault</span></span>|<span data-ttu-id="11304-112">нуль</span><span class="sxs-lookup"><span data-stu-id="11304-112">0</span></span>|<span data-ttu-id="11304-113">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="11304-113">PUA Protection is off.</span></span> <span data-ttu-id="11304-114">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="11304-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="11304-115">блок</span><span class="sxs-lookup"><span data-stu-id="11304-115">block</span></span>|<span data-ttu-id="11304-116">1,1</span><span class="sxs-lookup"><span data-stu-id="11304-116">1</span></span>|<span data-ttu-id="11304-117">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="11304-117">PUA Protection is on.</span></span> <span data-ttu-id="11304-118">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="11304-118">Detected items are blocked.</span></span> <span data-ttu-id="11304-119">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="11304-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="11304-120">включить</span><span class="sxs-lookup"><span data-stu-id="11304-120">audit</span></span>|<span data-ttu-id="11304-121">2</span><span class="sxs-lookup"><span data-stu-id="11304-121">2</span></span>|<span data-ttu-id="11304-122">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="11304-122">Audit mode.</span></span> <span data-ttu-id="11304-123">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="11304-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="11304-124">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="11304-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|



