---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a05aafa9a14399191adedc6c083ee371fe090a7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970936"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="7343c-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="7343c-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="7343c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7343c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7343c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7343c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7343c-106">Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="7343c-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="7343c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7343c-107">Members</span></span>
|<span data-ttu-id="7343c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7343c-108">Member</span></span>|<span data-ttu-id="7343c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7343c-109">Value</span></span>|<span data-ttu-id="7343c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7343c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7343c-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="7343c-111">deviceDefault</span></span>|<span data-ttu-id="7343c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7343c-112">0</span></span>|<span data-ttu-id="7343c-113">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="7343c-113">PUA Protection is off.</span></span> <span data-ttu-id="7343c-114">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="7343c-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="7343c-115">блок</span><span class="sxs-lookup"><span data-stu-id="7343c-115">block</span></span>|<span data-ttu-id="7343c-116">1,1</span><span class="sxs-lookup"><span data-stu-id="7343c-116">1</span></span>|<span data-ttu-id="7343c-117">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="7343c-117">PUA Protection is on.</span></span> <span data-ttu-id="7343c-118">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="7343c-118">Detected items are blocked.</span></span> <span data-ttu-id="7343c-119">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="7343c-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="7343c-120">включить</span><span class="sxs-lookup"><span data-stu-id="7343c-120">audit</span></span>|<span data-ttu-id="7343c-121">2</span><span class="sxs-lookup"><span data-stu-id="7343c-121">2</span></span>|<span data-ttu-id="7343c-122">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="7343c-122">Audit mode.</span></span> <span data-ttu-id="7343c-123">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="7343c-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="7343c-124">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="7343c-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





