---
title: Тип перечисления defenderMonitorFileActivity
description: Возможные значения для наблюдение за активностью файла.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d7b6c921ec40b53339646b2b3b0a91e2d4e8a84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837907"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="84aec-103">Тип перечисления defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="84aec-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="84aec-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84aec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84aec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84aec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84aec-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84aec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84aec-107">Возможные значения для наблюдение за активностью файла.</span><span class="sxs-lookup"><span data-stu-id="84aec-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="84aec-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="84aec-108">Members</span></span>
|<span data-ttu-id="84aec-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="84aec-109">Member</span></span>|<span data-ttu-id="84aec-110">Значение</span><span class="sxs-lookup"><span data-stu-id="84aec-110">Value</span></span>|<span data-ttu-id="84aec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84aec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84aec-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="84aec-112">userDefined</span></span>|<span data-ttu-id="84aec-113">0</span><span class="sxs-lookup"><span data-stu-id="84aec-113">0</span></span>|<span data-ttu-id="84aec-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="84aec-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="84aec-115">disable</span><span class="sxs-lookup"><span data-stu-id="84aec-115">disable</span></span>|<span data-ttu-id="84aec-116">1</span><span class="sxs-lookup"><span data-stu-id="84aec-116">1</span></span>|<span data-ttu-id="84aec-117">Отключение мониторинга активности файла.</span><span class="sxs-lookup"><span data-stu-id="84aec-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="84aec-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="84aec-118">monitorAllFiles</span></span>|<span data-ttu-id="84aec-119">2</span><span class="sxs-lookup"><span data-stu-id="84aec-119">2</span></span>|<span data-ttu-id="84aec-120">Отслеживать все файлы.</span><span class="sxs-lookup"><span data-stu-id="84aec-120">Monitor all files.</span></span>|
|<span data-ttu-id="84aec-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="84aec-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="84aec-122">3</span><span class="sxs-lookup"><span data-stu-id="84aec-122">3</span></span>| <span data-ttu-id="84aec-123">Отслеживание только входящих файлов.</span><span class="sxs-lookup"><span data-stu-id="84aec-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="84aec-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="84aec-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="84aec-125">4</span><span class="sxs-lookup"><span data-stu-id="84aec-125">4</span></span>|<span data-ttu-id="84aec-126">Мониторинг только исходящих файлов.</span><span class="sxs-lookup"><span data-stu-id="84aec-126">Monitor outgoing files only.</span></span>|





