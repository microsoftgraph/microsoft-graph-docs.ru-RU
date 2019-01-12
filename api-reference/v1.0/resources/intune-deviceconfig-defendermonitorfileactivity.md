---
title: Тип перечисления defenderMonitorFileActivity
description: Возможные значения для наблюдение за активностью файла.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d818264470543d077384f055cf2ef4004e019b26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937119"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="47d7e-103">Тип перечисления defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="47d7e-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="47d7e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47d7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47d7e-105">Возможные значения для наблюдение за активностью файла.</span><span class="sxs-lookup"><span data-stu-id="47d7e-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="47d7e-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="47d7e-106">Members</span></span>
|<span data-ttu-id="47d7e-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="47d7e-107">Member</span></span>|<span data-ttu-id="47d7e-108">Значение</span><span class="sxs-lookup"><span data-stu-id="47d7e-108">Value</span></span>|<span data-ttu-id="47d7e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="47d7e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d7e-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="47d7e-110">userDefined</span></span>|<span data-ttu-id="47d7e-111">0</span><span class="sxs-lookup"><span data-stu-id="47d7e-111">0</span></span>|<span data-ttu-id="47d7e-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="47d7e-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="47d7e-113">disable</span><span class="sxs-lookup"><span data-stu-id="47d7e-113">disable</span></span>|<span data-ttu-id="47d7e-114">1</span><span class="sxs-lookup"><span data-stu-id="47d7e-114">1</span></span>|<span data-ttu-id="47d7e-115">Отключение мониторинга активности файла.</span><span class="sxs-lookup"><span data-stu-id="47d7e-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="47d7e-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="47d7e-116">monitorAllFiles</span></span>|<span data-ttu-id="47d7e-117">2</span><span class="sxs-lookup"><span data-stu-id="47d7e-117">2</span></span>|<span data-ttu-id="47d7e-118">Отслеживать все файлы.</span><span class="sxs-lookup"><span data-stu-id="47d7e-118">Monitor all files.</span></span>|
|<span data-ttu-id="47d7e-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="47d7e-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="47d7e-120">3</span><span class="sxs-lookup"><span data-stu-id="47d7e-120">3</span></span>| <span data-ttu-id="47d7e-121">Отслеживание только входящих файлов.</span><span class="sxs-lookup"><span data-stu-id="47d7e-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="47d7e-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="47d7e-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="47d7e-123">4</span><span class="sxs-lookup"><span data-stu-id="47d7e-123">4</span></span>|<span data-ttu-id="47d7e-124">Мониторинг только исходящих файлов.</span><span class="sxs-lookup"><span data-stu-id="47d7e-124">Monitor outgoing files only.</span></span>|



