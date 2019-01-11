---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b3d496d6890d0da4d817ad9ba1f03e4b0825204d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861679"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="92c38-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="92c38-103">complianceState enum type</span></span>

> <span data-ttu-id="92c38-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="92c38-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92c38-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92c38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92c38-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="92c38-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92c38-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="92c38-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="92c38-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="92c38-108">Members</span></span>
|<span data-ttu-id="92c38-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="92c38-109">Member</span></span>|<span data-ttu-id="92c38-110">Значение</span><span class="sxs-lookup"><span data-stu-id="92c38-110">Value</span></span>|<span data-ttu-id="92c38-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92c38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c38-112">unknown</span><span class="sxs-lookup"><span data-stu-id="92c38-112">unknown</span></span>|<span data-ttu-id="92c38-113">0</span><span class="sxs-lookup"><span data-stu-id="92c38-113">0</span></span>|<span data-ttu-id="92c38-114">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="92c38-114">Unknown.</span></span>|
|<span data-ttu-id="92c38-115">спецификации</span><span class="sxs-lookup"><span data-stu-id="92c38-115">compliant</span></span>|<span data-ttu-id="92c38-116">1</span><span class="sxs-lookup"><span data-stu-id="92c38-116">1</span></span>|<span data-ttu-id="92c38-117">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="92c38-117">Compliant.</span></span>|
|<span data-ttu-id="92c38-118">несовместимый</span><span class="sxs-lookup"><span data-stu-id="92c38-118">noncompliant</span></span>|<span data-ttu-id="92c38-119">2</span><span class="sxs-lookup"><span data-stu-id="92c38-119">2</span></span>|<span data-ttu-id="92c38-120">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="92c38-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="92c38-121">конфликта</span><span class="sxs-lookup"><span data-stu-id="92c38-121">conflict</span></span>|<span data-ttu-id="92c38-122">3</span><span class="sxs-lookup"><span data-stu-id="92c38-122">3</span></span>|<span data-ttu-id="92c38-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="92c38-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="92c38-124">error</span><span class="sxs-lookup"><span data-stu-id="92c38-124">error</span></span>|<span data-ttu-id="92c38-125">4</span><span class="sxs-lookup"><span data-stu-id="92c38-125">4</span></span>|<span data-ttu-id="92c38-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="92c38-126">Error.</span></span>|
|<span data-ttu-id="92c38-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="92c38-127">inGracePeriod</span></span>|<span data-ttu-id="92c38-128">254</span><span class="sxs-lookup"><span data-stu-id="92c38-128">254</span></span>|<span data-ttu-id="92c38-129">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="92c38-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="92c38-130">configManager</span><span class="sxs-lookup"><span data-stu-id="92c38-130">configManager</span></span>|<span data-ttu-id="92c38-131">255</span><span class="sxs-lookup"><span data-stu-id="92c38-131">255</span></span>|<span data-ttu-id="92c38-132">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="92c38-132">Managed by Config Manager</span></span>|





