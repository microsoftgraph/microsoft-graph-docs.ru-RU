---
title: тип перечисления Дефендерпотентиаллюнвантедаппактион
description: Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aad2c9e37dfe3a3069caad25c7917a864c65a194
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256514"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="3c541-103">тип перечисления Дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="3c541-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

<span data-ttu-id="3c541-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c541-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c541-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c541-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c541-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c541-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c541-107">Действие защитника, которое будет принимать участие в обнаруженном потенциально нежелательном приложении (ПУА).</span><span class="sxs-lookup"><span data-stu-id="3c541-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="3c541-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3c541-108">Members</span></span>
|<span data-ttu-id="3c541-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3c541-109">Member</span></span>|<span data-ttu-id="3c541-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3c541-110">Value</span></span>|<span data-ttu-id="3c541-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c541-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c541-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="3c541-112">deviceDefault</span></span>|<span data-ttu-id="3c541-113">нуль</span><span class="sxs-lookup"><span data-stu-id="3c541-113">0</span></span>|<span data-ttu-id="3c541-114">Защита от Пуа отключена.</span><span class="sxs-lookup"><span data-stu-id="3c541-114">PUA Protection is off.</span></span> <span data-ttu-id="3c541-115">Защитник не будет защищаться от потенциально нежелательных приложений.</span><span class="sxs-lookup"><span data-stu-id="3c541-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="3c541-116">блок</span><span class="sxs-lookup"><span data-stu-id="3c541-116">block</span></span>|<span data-ttu-id="3c541-117">1,1</span><span class="sxs-lookup"><span data-stu-id="3c541-117">1</span></span>|<span data-ttu-id="3c541-118">Включена защита Пуа.</span><span class="sxs-lookup"><span data-stu-id="3c541-118">PUA Protection is on.</span></span> <span data-ttu-id="3c541-119">Обнаруженные элементы блокируются.</span><span class="sxs-lookup"><span data-stu-id="3c541-119">Detected items are blocked.</span></span> <span data-ttu-id="3c541-120">Они будут отображаться в журнале вместе с другими угрозами.</span><span class="sxs-lookup"><span data-stu-id="3c541-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="3c541-121">включить</span><span class="sxs-lookup"><span data-stu-id="3c541-121">audit</span></span>|<span data-ttu-id="3c541-122">2</span><span class="sxs-lookup"><span data-stu-id="3c541-122">2</span></span>|<span data-ttu-id="3c541-123">Режим аудита.</span><span class="sxs-lookup"><span data-stu-id="3c541-123">Audit mode.</span></span> <span data-ttu-id="3c541-124">Защитник обнаружит потенциально нежелательные приложения, но не выполнит никаких действий.</span><span class="sxs-lookup"><span data-stu-id="3c541-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="3c541-125">Чтобы просмотреть сведения о защитнике приложений, необходимо выполнить поиск событий, созданных защитником, в средстве просмотра событий.</span><span class="sxs-lookup"><span data-stu-id="3c541-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




