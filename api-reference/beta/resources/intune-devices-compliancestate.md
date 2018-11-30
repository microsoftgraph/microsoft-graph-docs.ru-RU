---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
ms.openlocfilehash: c49c0ecc2511f612e743fb5d86a53d150d3fbf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081093"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="b9c8d-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="b9c8d-103">complianceState enum type</span></span>

> <span data-ttu-id="b9c8d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9c8d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9c8d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9c8d-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="b9c8d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b9c8d-108">Members</span></span>
|<span data-ttu-id="b9c8d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b9c8d-109">Member</span></span>|<span data-ttu-id="b9c8d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b9c8d-110">Value</span></span>|<span data-ttu-id="b9c8d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9c8d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="b9c8d-112">unknown</span></span>|<span data-ttu-id="b9c8d-113">0</span><span class="sxs-lookup"><span data-stu-id="b9c8d-113">0</span></span>|<span data-ttu-id="b9c8d-114">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-114">Unknown.</span></span>|
|<span data-ttu-id="b9c8d-115">спецификации</span><span class="sxs-lookup"><span data-stu-id="b9c8d-115">compliant</span></span>|<span data-ttu-id="b9c8d-116">1</span><span class="sxs-lookup"><span data-stu-id="b9c8d-116">1</span></span>|<span data-ttu-id="b9c8d-117">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-117">Compliant.</span></span>|
|<span data-ttu-id="b9c8d-118">несовместимый</span><span class="sxs-lookup"><span data-stu-id="b9c8d-118">noncompliant</span></span>|<span data-ttu-id="b9c8d-119">2</span><span class="sxs-lookup"><span data-stu-id="b9c8d-119">2</span></span>|<span data-ttu-id="b9c8d-120">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="b9c8d-121">конфликта</span><span class="sxs-lookup"><span data-stu-id="b9c8d-121">conflict</span></span>|<span data-ttu-id="b9c8d-122">3</span><span class="sxs-lookup"><span data-stu-id="b9c8d-122">3</span></span>|<span data-ttu-id="b9c8d-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="b9c8d-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="b9c8d-124">error</span><span class="sxs-lookup"><span data-stu-id="b9c8d-124">error</span></span>|<span data-ttu-id="b9c8d-125">4</span><span class="sxs-lookup"><span data-stu-id="b9c8d-125">4</span></span>|<span data-ttu-id="b9c8d-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="b9c8d-126">Error.</span></span>|
|<span data-ttu-id="b9c8d-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="b9c8d-127">inGracePeriod</span></span>|<span data-ttu-id="b9c8d-128">254</span><span class="sxs-lookup"><span data-stu-id="b9c8d-128">254</span></span>|<span data-ttu-id="b9c8d-129">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="b9c8d-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="b9c8d-130">configManager</span><span class="sxs-lookup"><span data-stu-id="b9c8d-130">configManager</span></span>|<span data-ttu-id="b9c8d-131">255</span><span class="sxs-lookup"><span data-stu-id="b9c8d-131">255</span></span>|<span data-ttu-id="b9c8d-132">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="b9c8d-132">Managed by Config Manager</span></span>|





