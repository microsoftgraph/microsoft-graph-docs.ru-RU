---
title: Тип перечисления windowsUpdateStatus
description: Для бизнеса конфигурации устройства состояний центра обновления Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431744"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="289be-103">Тип перечисления windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="289be-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="289be-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="289be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="289be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="289be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="289be-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="289be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="289be-107">Для бизнеса конфигурации устройства состояний центра обновления Windows</span><span class="sxs-lookup"><span data-stu-id="289be-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="289be-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="289be-108">Members</span></span>
|<span data-ttu-id="289be-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="289be-109">Member</span></span>|<span data-ttu-id="289be-110">Значение</span><span class="sxs-lookup"><span data-stu-id="289be-110">Value</span></span>|<span data-ttu-id="289be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="289be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="289be-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="289be-112">upToDate</span></span>|<span data-ttu-id="289be-113">0</span><span class="sxs-lookup"><span data-stu-id="289be-113">0</span></span>|<span data-ttu-id="289be-114">Отсутствуют ожидающие обновления, не ожидающие обновления перезагрузку и не сбоя обновления.</span><span class="sxs-lookup"><span data-stu-id="289be-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="289be-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="289be-115">pendingInstallation</span></span>|<span data-ttu-id="289be-116">1</span><span class="sxs-lookup"><span data-stu-id="289be-116">1</span></span>|<span data-ttu-id="289be-117">Существует обновлений, ожидающих установки, включающий обновлений, которые не утверждено.</span><span class="sxs-lookup"><span data-stu-id="289be-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="289be-118">Существует обновления не ожидается перезагрузка, не сбоя обновления.</span><span class="sxs-lookup"><span data-stu-id="289be-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="289be-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="289be-119">pendingReboot</span></span>|<span data-ttu-id="289be-120">2</span><span class="sxs-lookup"><span data-stu-id="289be-120">2</span></span>|<span data-ttu-id="289be-121">Существует обновлений, которые необходимо перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="289be-121">There are updates that requires reboot.</span></span> <span data-ttu-id="289be-122">Не неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="289be-122">There are not failed updates.</span></span>|
|<span data-ttu-id="289be-123">failed</span><span class="sxs-lookup"><span data-stu-id="289be-123">failed</span></span>|<span data-ttu-id="289be-124">3</span><span class="sxs-lookup"><span data-stu-id="289be-124">3</span></span>|<span data-ttu-id="289be-125">Есть обновления не удается установить на устройстве.</span><span class="sxs-lookup"><span data-stu-id="289be-125">There are updates failed to install on the device.</span></span>|




