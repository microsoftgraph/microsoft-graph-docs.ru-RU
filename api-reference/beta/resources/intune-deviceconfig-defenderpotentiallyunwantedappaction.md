---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально неЖелательном приложении (ПУА).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1949ec58c7cfd2d896308f740b7eca16f2646b3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534810"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="37cf6-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="37cf6-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="37cf6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37cf6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37cf6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37cf6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37cf6-106">Действие защитника, которое будет принимать участие в обнаруженном потенциально неЖелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="37cf6-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="37cf6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="37cf6-107">Members</span></span>
|<span data-ttu-id="37cf6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="37cf6-108">Member</span></span>|<span data-ttu-id="37cf6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="37cf6-109">Value</span></span>|<span data-ttu-id="37cf6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="37cf6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37cf6-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="37cf6-111">deviceDefault</span></span>|<span data-ttu-id="37cf6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="37cf6-112">0</span></span>|<span data-ttu-id="37cf6-113">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="37cf6-113">PUA Protection is off.</span></span> <span data-ttu-id="37cf6-114">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="37cf6-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="37cf6-115">блок</span><span class="sxs-lookup"><span data-stu-id="37cf6-115">block</span></span>|<span data-ttu-id="37cf6-116">1 </span><span class="sxs-lookup"><span data-stu-id="37cf6-116">1</span></span>|<span data-ttu-id="37cf6-117">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="37cf6-117">PUA Protection is on.</span></span> <span data-ttu-id="37cf6-118">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="37cf6-118">Detected items are blocked.</span></span> <span data-ttu-id="37cf6-119">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="37cf6-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="37cf6-120">включить</span><span class="sxs-lookup"><span data-stu-id="37cf6-120">audit</span></span>|<span data-ttu-id="37cf6-121">2 </span><span class="sxs-lookup"><span data-stu-id="37cf6-121">2</span></span>|<span data-ttu-id="37cf6-122">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="37cf6-122">Audit mode.</span></span> <span data-ttu-id="37cf6-123">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="37cf6-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="37cf6-124">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="37cf6-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





