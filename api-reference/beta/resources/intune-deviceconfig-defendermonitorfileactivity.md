---
title: Тип перечисления defenderMonitorFileActivity
description: Возможные значения для наблюдение за активностью файла.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: df973c06456484263b6346b5eaa48ac466de41f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967996"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="b74f3-103">Тип перечисления defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b74f3-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="b74f3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b74f3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b74f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b74f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b74f3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b74f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b74f3-107">Возможные значения для наблюдение за активностью файла.</span><span class="sxs-lookup"><span data-stu-id="b74f3-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="b74f3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b74f3-108">Members</span></span>
|<span data-ttu-id="b74f3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b74f3-109">Member</span></span>|<span data-ttu-id="b74f3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b74f3-110">Value</span></span>|<span data-ttu-id="b74f3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b74f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b74f3-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="b74f3-112">userDefined</span></span>|<span data-ttu-id="b74f3-113">0</span><span class="sxs-lookup"><span data-stu-id="b74f3-113">0</span></span>|<span data-ttu-id="b74f3-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="b74f3-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b74f3-115">disable</span><span class="sxs-lookup"><span data-stu-id="b74f3-115">disable</span></span>|<span data-ttu-id="b74f3-116">1</span><span class="sxs-lookup"><span data-stu-id="b74f3-116">1</span></span>|<span data-ttu-id="b74f3-117">Отключение мониторинга активности файла.</span><span class="sxs-lookup"><span data-stu-id="b74f3-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="b74f3-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="b74f3-118">monitorAllFiles</span></span>|<span data-ttu-id="b74f3-119">2</span><span class="sxs-lookup"><span data-stu-id="b74f3-119">2</span></span>|<span data-ttu-id="b74f3-120">Отслеживать все файлы.</span><span class="sxs-lookup"><span data-stu-id="b74f3-120">Monitor all files.</span></span>|
|<span data-ttu-id="b74f3-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="b74f3-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="b74f3-122">3</span><span class="sxs-lookup"><span data-stu-id="b74f3-122">3</span></span>| <span data-ttu-id="b74f3-123">Отслеживание только входящих файлов.</span><span class="sxs-lookup"><span data-stu-id="b74f3-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="b74f3-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="b74f3-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="b74f3-125">4</span><span class="sxs-lookup"><span data-stu-id="b74f3-125">4</span></span>|<span data-ttu-id="b74f3-126">Мониторинг только исходящих файлов.</span><span class="sxs-lookup"><span data-stu-id="b74f3-126">Monitor outgoing files only.</span></span>|





