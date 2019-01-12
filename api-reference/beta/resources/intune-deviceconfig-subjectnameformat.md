---
title: Тип перечисления subjectNameFormat
description: Параметры формата имени субъекта.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 259af745567a0fc5de004f5a804d8bab00355f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969592"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="55ec8-103">Тип перечисления subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="55ec8-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="55ec8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="55ec8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55ec8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ec8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55ec8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55ec8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55ec8-107">Параметры формата имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="55ec8-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="55ec8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="55ec8-108">Members</span></span>
|<span data-ttu-id="55ec8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="55ec8-109">Member</span></span>|<span data-ttu-id="55ec8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="55ec8-110">Value</span></span>|<span data-ttu-id="55ec8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55ec8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ec8-112">_ общего _ имени</span><span class="sxs-lookup"><span data-stu-id="55ec8-112">commonName</span></span>|<span data-ttu-id="55ec8-113">0</span><span class="sxs-lookup"><span data-stu-id="55ec8-113">0</span></span>|<span data-ttu-id="55ec8-114">Общее имя.</span><span class="sxs-lookup"><span data-stu-id="55ec8-114">Common name.</span></span>|
|<span data-ttu-id="55ec8-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="55ec8-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="55ec8-116">1</span><span class="sxs-lookup"><span data-stu-id="55ec8-116">1</span></span>|<span data-ttu-id="55ec8-117">Общее имя, включая электронной почты.</span><span class="sxs-lookup"><span data-stu-id="55ec8-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="55ec8-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="55ec8-118">commonNameAsEmail</span></span>|<span data-ttu-id="55ec8-119">2</span><span class="sxs-lookup"><span data-stu-id="55ec8-119">2</span></span>|<span data-ttu-id="55ec8-120">Общее имя по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="55ec8-120">Common Name As Email.</span></span>|
|<span data-ttu-id="55ec8-121">custom</span><span class="sxs-lookup"><span data-stu-id="55ec8-121">custom</span></span>|<span data-ttu-id="55ec8-122">3</span><span class="sxs-lookup"><span data-stu-id="55ec8-122">3</span></span>|<span data-ttu-id="55ec8-123">Формат имени настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="55ec8-123">Custom subject name format.</span></span>|
|<span data-ttu-id="55ec8-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="55ec8-124">commonNameAsIMEI</span></span>|<span data-ttu-id="55ec8-125">5</span><span class="sxs-lookup"><span data-stu-id="55ec8-125">5</span></span>|<span data-ttu-id="55ec8-126">Общее имя как IMEI.</span><span class="sxs-lookup"><span data-stu-id="55ec8-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="55ec8-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="55ec8-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="55ec8-128">6</span><span class="sxs-lookup"><span data-stu-id="55ec8-128">6</span></span>|<span data-ttu-id="55ec8-129">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="55ec8-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="55ec8-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="55ec8-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="55ec8-131">7</span><span class="sxs-lookup"><span data-stu-id="55ec8-131">7</span></span>|<span data-ttu-id="55ec8-132">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="55ec8-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="55ec8-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="55ec8-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="55ec8-134">8</span><span class="sxs-lookup"><span data-stu-id="55ec8-134">8</span></span>|<span data-ttu-id="55ec8-135">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="55ec8-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="55ec8-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="55ec8-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="55ec8-137">9</span><span class="sxs-lookup"><span data-stu-id="55ec8-137">9</span></span>|<span data-ttu-id="55ec8-138">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="55ec8-138">Common Name As Serial Number.</span></span>|





