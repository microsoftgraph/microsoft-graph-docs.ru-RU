---
title: Тип перечисления defenderMonitorFileActivity
description: Возможные значения для наблюдение за активностью файла.
ms.openlocfilehash: ec10458cbb76a45caff8d64f6c4047d5645094b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080407"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="b37df-103">Тип перечисления defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b37df-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="b37df-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b37df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b37df-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b37df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b37df-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b37df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b37df-107">Возможные значения для наблюдение за активностью файла.</span><span class="sxs-lookup"><span data-stu-id="b37df-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="b37df-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b37df-108">Members</span></span>
|<span data-ttu-id="b37df-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b37df-109">Member</span></span>|<span data-ttu-id="b37df-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b37df-110">Value</span></span>|<span data-ttu-id="b37df-111">Description</span><span class="sxs-lookup"><span data-stu-id="b37df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b37df-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="b37df-112">userDefined</span></span>|<span data-ttu-id="b37df-113">0</span><span class="sxs-lookup"><span data-stu-id="b37df-113">0</span></span>|<span data-ttu-id="b37df-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="b37df-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b37df-115">Отключение</span><span class="sxs-lookup"><span data-stu-id="b37df-115">disable</span></span>|<span data-ttu-id="b37df-116">1</span><span class="sxs-lookup"><span data-stu-id="b37df-116">1</span></span>|<span data-ttu-id="b37df-117">Отключение мониторинга активности файла.</span><span class="sxs-lookup"><span data-stu-id="b37df-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="b37df-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="b37df-118">monitorAllFiles</span></span>|<span data-ttu-id="b37df-119">2</span><span class="sxs-lookup"><span data-stu-id="b37df-119">2</span></span>|<span data-ttu-id="b37df-120">Отслеживать все файлы.</span><span class="sxs-lookup"><span data-stu-id="b37df-120">Monitor all files.</span></span>|
|<span data-ttu-id="b37df-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="b37df-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="b37df-122">3</span><span class="sxs-lookup"><span data-stu-id="b37df-122">3</span></span>| <span data-ttu-id="b37df-123">Отслеживание только входящих файлов.</span><span class="sxs-lookup"><span data-stu-id="b37df-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="b37df-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="b37df-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="b37df-125">4</span><span class="sxs-lookup"><span data-stu-id="b37df-125">4</span></span>|<span data-ttu-id="b37df-126">Мониторинг только исходящих файлов.</span><span class="sxs-lookup"><span data-stu-id="b37df-126">Monitor outgoing files only.</span></span>|





