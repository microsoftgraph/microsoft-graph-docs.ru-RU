---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4eeadad81c86217048590cff73a212e830e1f94f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526887"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="4d20e-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="4d20e-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

<span data-ttu-id="4d20e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d20e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d20e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d20e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d20e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d20e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d20e-107">Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="4d20e-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="4d20e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4d20e-108">Members</span></span>
|<span data-ttu-id="4d20e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4d20e-109">Member</span></span>|<span data-ttu-id="4d20e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4d20e-110">Value</span></span>|<span data-ttu-id="4d20e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4d20e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d20e-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="4d20e-112">deviceDefault</span></span>|<span data-ttu-id="4d20e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4d20e-113">0</span></span>|<span data-ttu-id="4d20e-114">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="4d20e-114">PUA Protection is off.</span></span> <span data-ttu-id="4d20e-115">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="4d20e-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="4d20e-116">блок</span><span class="sxs-lookup"><span data-stu-id="4d20e-116">block</span></span>|<span data-ttu-id="4d20e-117">1 </span><span class="sxs-lookup"><span data-stu-id="4d20e-117">1</span></span>|<span data-ttu-id="4d20e-118">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="4d20e-118">PUA Protection is on.</span></span> <span data-ttu-id="4d20e-119">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="4d20e-119">Detected items are blocked.</span></span> <span data-ttu-id="4d20e-120">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="4d20e-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="4d20e-121">включить</span><span class="sxs-lookup"><span data-stu-id="4d20e-121">audit</span></span>|<span data-ttu-id="4d20e-122">2 </span><span class="sxs-lookup"><span data-stu-id="4d20e-122">2</span></span>|<span data-ttu-id="4d20e-123">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="4d20e-123">Audit mode.</span></span> <span data-ttu-id="4d20e-124">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="4d20e-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="4d20e-125">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="4d20e-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|



