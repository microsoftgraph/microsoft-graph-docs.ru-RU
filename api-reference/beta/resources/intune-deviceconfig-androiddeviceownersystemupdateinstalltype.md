---
title: Тип перечисления androidDeviceOwnerSystemUpdateInstallType
description: Системные типы обновлений для Android устройства владельцем.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9a46d60972bab46fa0e2cda8d03a090bd8b810a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980974"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="b45af-103">Тип перечисления androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="b45af-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="b45af-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b45af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b45af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b45af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b45af-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b45af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b45af-107">Системные типы обновлений для Android устройства владельцем.</span><span class="sxs-lookup"><span data-stu-id="b45af-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="b45af-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b45af-108">Members</span></span>
|<span data-ttu-id="b45af-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b45af-109">Member</span></span>|<span data-ttu-id="b45af-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b45af-110">Value</span></span>|<span data-ttu-id="b45af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b45af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b45af-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b45af-112">deviceDefault</span></span>|<span data-ttu-id="b45af-113">0</span><span class="sxs-lookup"><span data-stu-id="b45af-113">0</span></span>|<span data-ttu-id="b45af-114">Поведение по умолчанию устройство, которое обычно выдает запрос пользователю принимать обновления системы.</span><span class="sxs-lookup"><span data-stu-id="b45af-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="b45af-115">отложить</span><span class="sxs-lookup"><span data-stu-id="b45af-115">postpone</span></span>|<span data-ttu-id="b45af-116">1</span><span class="sxs-lookup"><span data-stu-id="b45af-116">1</span></span>|<span data-ttu-id="b45af-117">Отложить автоматическую установку обновлений вверх до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="b45af-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="b45af-118">оконного</span><span class="sxs-lookup"><span data-stu-id="b45af-118">windowed</span></span>|<span data-ttu-id="b45af-119">2</span><span class="sxs-lookup"><span data-stu-id="b45af-119">2</span></span>|<span data-ttu-id="b45af-120">Внутри ежедневного периода обслуживания автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="b45af-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="b45af-121">Автоматически</span><span class="sxs-lookup"><span data-stu-id="b45af-121">automatic</span></span>|<span data-ttu-id="b45af-122">3</span><span class="sxs-lookup"><span data-stu-id="b45af-122">3</span></span>|<span data-ttu-id="b45af-123">Как можно скорее автоматическую установку обновлений.</span><span class="sxs-lookup"><span data-stu-id="b45af-123">Automatically install updates as soon as possible.</span></span>|





