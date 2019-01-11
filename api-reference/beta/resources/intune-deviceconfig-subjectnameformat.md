---
title: Тип перечисления subjectNameFormat
description: Параметры формата имени субъекта.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 85a11e8690c360e405df2453229a039ea9f9b1dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821338"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="62ff0-103">Тип перечисления subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62ff0-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="62ff0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62ff0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62ff0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62ff0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62ff0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62ff0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62ff0-107">Параметры формата имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="62ff0-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="62ff0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="62ff0-108">Members</span></span>
|<span data-ttu-id="62ff0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="62ff0-109">Member</span></span>|<span data-ttu-id="62ff0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="62ff0-110">Value</span></span>|<span data-ttu-id="62ff0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="62ff0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62ff0-112">_ общего _ имени</span><span class="sxs-lookup"><span data-stu-id="62ff0-112">commonName</span></span>|<span data-ttu-id="62ff0-113">0</span><span class="sxs-lookup"><span data-stu-id="62ff0-113">0</span></span>|<span data-ttu-id="62ff0-114">Общее имя.</span><span class="sxs-lookup"><span data-stu-id="62ff0-114">Common name.</span></span>|
|<span data-ttu-id="62ff0-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="62ff0-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="62ff0-116">1</span><span class="sxs-lookup"><span data-stu-id="62ff0-116">1</span></span>|<span data-ttu-id="62ff0-117">Общее имя, включая электронной почты.</span><span class="sxs-lookup"><span data-stu-id="62ff0-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="62ff0-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="62ff0-118">commonNameAsEmail</span></span>|<span data-ttu-id="62ff0-119">2</span><span class="sxs-lookup"><span data-stu-id="62ff0-119">2</span></span>|<span data-ttu-id="62ff0-120">Общее имя по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="62ff0-120">Common Name As Email.</span></span>|
|<span data-ttu-id="62ff0-121">custom</span><span class="sxs-lookup"><span data-stu-id="62ff0-121">custom</span></span>|<span data-ttu-id="62ff0-122">3</span><span class="sxs-lookup"><span data-stu-id="62ff0-122">3</span></span>|<span data-ttu-id="62ff0-123">Формат имени настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="62ff0-123">Custom subject name format.</span></span>|
|<span data-ttu-id="62ff0-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="62ff0-124">commonNameAsIMEI</span></span>|<span data-ttu-id="62ff0-125">5</span><span class="sxs-lookup"><span data-stu-id="62ff0-125">5</span></span>|<span data-ttu-id="62ff0-126">Общее имя как IMEI.</span><span class="sxs-lookup"><span data-stu-id="62ff0-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="62ff0-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="62ff0-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="62ff0-128">6</span><span class="sxs-lookup"><span data-stu-id="62ff0-128">6</span></span>|<span data-ttu-id="62ff0-129">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="62ff0-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="62ff0-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="62ff0-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="62ff0-131">7</span><span class="sxs-lookup"><span data-stu-id="62ff0-131">7</span></span>|<span data-ttu-id="62ff0-132">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="62ff0-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="62ff0-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="62ff0-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="62ff0-134">8</span><span class="sxs-lookup"><span data-stu-id="62ff0-134">8</span></span>|<span data-ttu-id="62ff0-135">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="62ff0-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="62ff0-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="62ff0-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="62ff0-137">9</span><span class="sxs-lookup"><span data-stu-id="62ff0-137">9</span></span>|<span data-ttu-id="62ff0-138">Общее имя как серийный номер.</span><span class="sxs-lookup"><span data-stu-id="62ff0-138">Common Name As Serial Number.</span></span>|





