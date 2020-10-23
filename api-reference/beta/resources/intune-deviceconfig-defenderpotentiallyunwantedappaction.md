---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2919edb11cc29f8a78d3bde32808f285eef25b4c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696358"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="1307c-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="1307c-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

<span data-ttu-id="1307c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1307c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1307c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1307c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1307c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1307c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1307c-107">Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="1307c-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="1307c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1307c-108">Members</span></span>
|<span data-ttu-id="1307c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1307c-109">Member</span></span>|<span data-ttu-id="1307c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1307c-110">Value</span></span>|<span data-ttu-id="1307c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1307c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1307c-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="1307c-112">deviceDefault</span></span>|<span data-ttu-id="1307c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1307c-113">0</span></span>|<span data-ttu-id="1307c-114">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="1307c-114">PUA Protection is off.</span></span> <span data-ttu-id="1307c-115">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="1307c-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="1307c-116">блок</span><span class="sxs-lookup"><span data-stu-id="1307c-116">block</span></span>|<span data-ttu-id="1307c-117">1,1</span><span class="sxs-lookup"><span data-stu-id="1307c-117">1</span></span>|<span data-ttu-id="1307c-118">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="1307c-118">PUA Protection is on.</span></span> <span data-ttu-id="1307c-119">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="1307c-119">Detected items are blocked.</span></span> <span data-ttu-id="1307c-120">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="1307c-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="1307c-121">включить</span><span class="sxs-lookup"><span data-stu-id="1307c-121">audit</span></span>|<span data-ttu-id="1307c-122">2</span><span class="sxs-lookup"><span data-stu-id="1307c-122">2</span></span>|<span data-ttu-id="1307c-123">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="1307c-123">Audit mode.</span></span> <span data-ttu-id="1307c-124">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="1307c-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="1307c-125">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="1307c-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





