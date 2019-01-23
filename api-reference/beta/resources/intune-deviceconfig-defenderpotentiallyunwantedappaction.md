---
title: Тип перечисления defenderPotentiallyUnwantedAppAction
description: Защитника действие, которое выполняется обнаруженных потенциально ненужные приложения (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422756"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="c20e8-103">Тип перечисления defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="c20e8-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="c20e8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c20e8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c20e8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c20e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c20e8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c20e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c20e8-107">Защитника действие, которое выполняется обнаруженных потенциально ненужные приложения (PUA).</span><span class="sxs-lookup"><span data-stu-id="c20e8-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="c20e8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c20e8-108">Members</span></span>
|<span data-ttu-id="c20e8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c20e8-109">Member</span></span>|<span data-ttu-id="c20e8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c20e8-110">Value</span></span>|<span data-ttu-id="c20e8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c20e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c20e8-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c20e8-112">deviceDefault</span></span>|<span data-ttu-id="c20e8-113">0</span><span class="sxs-lookup"><span data-stu-id="c20e8-113">0</span></span>|<span data-ttu-id="c20e8-114">Защита PUA отключено.</span><span class="sxs-lookup"><span data-stu-id="c20e8-114">PUA Protection is off.</span></span> <span data-ttu-id="c20e8-115">Защитник будет обеспечивает защиту от нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="c20e8-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="c20e8-116">блок</span><span class="sxs-lookup"><span data-stu-id="c20e8-116">block</span></span>|<span data-ttu-id="c20e8-117">1</span><span class="sxs-lookup"><span data-stu-id="c20e8-117">1</span></span>|<span data-ttu-id="c20e8-118">Защита от PUA включена.</span><span class="sxs-lookup"><span data-stu-id="c20e8-118">PUA Protection is on.</span></span> <span data-ttu-id="c20e8-119">Обнаруженными блокируются.</span><span class="sxs-lookup"><span data-stu-id="c20e8-119">Detected items are blocked.</span></span> <span data-ttu-id="c20e8-120">Они будут отображаться в журнал, а также другие угрозы, связанные с.</span><span class="sxs-lookup"><span data-stu-id="c20e8-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="c20e8-121">Аудит</span><span class="sxs-lookup"><span data-stu-id="c20e8-121">audit</span></span>|<span data-ttu-id="c20e8-122">2</span><span class="sxs-lookup"><span data-stu-id="c20e8-122">2</span></span>|<span data-ttu-id="c20e8-123">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="c20e8-123">Audit mode.</span></span> <span data-ttu-id="c20e8-124">Защитник обнаружения нежелательных приложений, но не действий.</span><span class="sxs-lookup"><span data-stu-id="c20e8-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="c20e8-125">Можно просмотреть сведения о приложениях Защитник бы вступили претензий поиск по ключевым словам для создания Защитником событий средства просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="c20e8-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




