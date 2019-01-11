---
title: Тип перечисления defenderPotentiallyUnwantedAppAction
description: Защитника действие, которое выполняется обнаруженных потенциально ненужные приложения (PUA).
localization_priority: Normal
ms.openlocfilehash: 9b04cd6daeae303910519d0735165171575d8c44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858648"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="956a3-103">Тип перечисления defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="956a3-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="956a3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="956a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="956a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="956a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="956a3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="956a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="956a3-107">Защитника действие, которое выполняется обнаруженных потенциально ненужные приложения (PUA).</span><span class="sxs-lookup"><span data-stu-id="956a3-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>
## <a name="members"></a><span data-ttu-id="956a3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="956a3-108">Members</span></span>
|<span data-ttu-id="956a3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="956a3-109">Member</span></span>|<span data-ttu-id="956a3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="956a3-110">Value</span></span>|<span data-ttu-id="956a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="956a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="956a3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="956a3-112">deviceDefault</span></span>|<span data-ttu-id="956a3-113">0</span><span class="sxs-lookup"><span data-stu-id="956a3-113">0</span></span>|<span data-ttu-id="956a3-114">Защита PUA отключено.</span><span class="sxs-lookup"><span data-stu-id="956a3-114">PUA Protection is off.</span></span> <span data-ttu-id="956a3-115">Защитник будет обеспечивает защиту от нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="956a3-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="956a3-116">блок</span><span class="sxs-lookup"><span data-stu-id="956a3-116">block</span></span>|<span data-ttu-id="956a3-117">1</span><span class="sxs-lookup"><span data-stu-id="956a3-117">1</span></span>|<span data-ttu-id="956a3-118">Защита от PUA включена.</span><span class="sxs-lookup"><span data-stu-id="956a3-118">PUA Protection is on.</span></span> <span data-ttu-id="956a3-119">Обнаруженными блокируются.</span><span class="sxs-lookup"><span data-stu-id="956a3-119">Detected items are blocked.</span></span> <span data-ttu-id="956a3-120">Они будут отображаться в журнал, а также другие угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="956a3-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="956a3-121">Аудит</span><span class="sxs-lookup"><span data-stu-id="956a3-121">audit</span></span>|<span data-ttu-id="956a3-122">2</span><span class="sxs-lookup"><span data-stu-id="956a3-122">2</span></span>|<span data-ttu-id="956a3-123">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="956a3-123">Audit mode.</span></span> <span data-ttu-id="956a3-124">Защитник обнаружения нежелательных приложений, но не действий.</span><span class="sxs-lookup"><span data-stu-id="956a3-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="956a3-125">Можно просмотреть сведения о приложениях Защитник бы вступили претензий поиск по ключевым словам для создания Защитником событий средства просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="956a3-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





