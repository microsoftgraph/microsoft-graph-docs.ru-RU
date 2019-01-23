---
title: Тип перечисления defenderMonitorFileActivity
description: Возможные значения для наблюдение за активностью файла.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9b0f91d0a2d802fd573d7825da016dc8850e941
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414958"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="0a6c7-103">Тип перечисления defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="0a6c7-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="0a6c7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0a6c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a6c7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a6c7-107">Возможные значения для наблюдение за активностью файла.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="0a6c7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0a6c7-108">Members</span></span>
|<span data-ttu-id="0a6c7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0a6c7-109">Member</span></span>|<span data-ttu-id="0a6c7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0a6c7-110">Value</span></span>|<span data-ttu-id="0a6c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a6c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a6c7-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="0a6c7-112">userDefined</span></span>|<span data-ttu-id="0a6c7-113">0</span><span class="sxs-lookup"><span data-stu-id="0a6c7-113">0</span></span>|<span data-ttu-id="0a6c7-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="0a6c7-115">Отключение</span><span class="sxs-lookup"><span data-stu-id="0a6c7-115">disable</span></span>|<span data-ttu-id="0a6c7-116">1</span><span class="sxs-lookup"><span data-stu-id="0a6c7-116">1</span></span>|<span data-ttu-id="0a6c7-117">Отключение мониторинга активности файла.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="0a6c7-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="0a6c7-118">monitorAllFiles</span></span>|<span data-ttu-id="0a6c7-119">2</span><span class="sxs-lookup"><span data-stu-id="0a6c7-119">2</span></span>|<span data-ttu-id="0a6c7-120">Отслеживать все файлы.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-120">Monitor all files.</span></span>|
|<span data-ttu-id="0a6c7-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="0a6c7-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="0a6c7-122">3</span><span class="sxs-lookup"><span data-stu-id="0a6c7-122">3</span></span>| <span data-ttu-id="0a6c7-123">Отслеживание только входящих файлов.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="0a6c7-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="0a6c7-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="0a6c7-125">4</span><span class="sxs-lookup"><span data-stu-id="0a6c7-125">4</span></span>|<span data-ttu-id="0a6c7-126">Мониторинг только исходящих файлов.</span><span class="sxs-lookup"><span data-stu-id="0a6c7-126">Monitor outgoing files only.</span></span>|




