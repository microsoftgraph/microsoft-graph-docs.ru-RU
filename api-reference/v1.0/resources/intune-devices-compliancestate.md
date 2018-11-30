---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
ms.openlocfilehash: 041a2267b952d37e0aeef29e1325e5cb7b561ed7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027853"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="21aa3-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="21aa3-103">complianceState enum type</span></span>

> <span data-ttu-id="21aa3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21aa3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21aa3-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="21aa3-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="21aa3-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="21aa3-106">Members</span></span>
|<span data-ttu-id="21aa3-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="21aa3-107">Member</span></span>|<span data-ttu-id="21aa3-108">Значение</span><span class="sxs-lookup"><span data-stu-id="21aa3-108">Value</span></span>|<span data-ttu-id="21aa3-109">Description</span><span class="sxs-lookup"><span data-stu-id="21aa3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21aa3-110">unknown</span><span class="sxs-lookup"><span data-stu-id="21aa3-110">unknown</span></span>|<span data-ttu-id="21aa3-111">0</span><span class="sxs-lookup"><span data-stu-id="21aa3-111">0</span></span>|<span data-ttu-id="21aa3-112">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="21aa3-112">Unknown.</span></span>|
|<span data-ttu-id="21aa3-113">спецификации</span><span class="sxs-lookup"><span data-stu-id="21aa3-113">compliant</span></span>|<span data-ttu-id="21aa3-114">1</span><span class="sxs-lookup"><span data-stu-id="21aa3-114">1</span></span>|<span data-ttu-id="21aa3-115">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="21aa3-115">Compliant.</span></span>|
|<span data-ttu-id="21aa3-116">несовместимый</span><span class="sxs-lookup"><span data-stu-id="21aa3-116">noncompliant</span></span>|<span data-ttu-id="21aa3-117">2</span><span class="sxs-lookup"><span data-stu-id="21aa3-117">2</span></span>|<span data-ttu-id="21aa3-118">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="21aa3-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="21aa3-119">конфликта</span><span class="sxs-lookup"><span data-stu-id="21aa3-119">conflict</span></span>|<span data-ttu-id="21aa3-120">3</span><span class="sxs-lookup"><span data-stu-id="21aa3-120">3</span></span>|<span data-ttu-id="21aa3-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="21aa3-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="21aa3-122">error</span><span class="sxs-lookup"><span data-stu-id="21aa3-122">error</span></span>|<span data-ttu-id="21aa3-123">4</span><span class="sxs-lookup"><span data-stu-id="21aa3-123">4</span></span>|<span data-ttu-id="21aa3-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="21aa3-124">Error.</span></span>|
|<span data-ttu-id="21aa3-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="21aa3-125">inGracePeriod</span></span>|<span data-ttu-id="21aa3-126">254</span><span class="sxs-lookup"><span data-stu-id="21aa3-126">254</span></span>|<span data-ttu-id="21aa3-127">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="21aa3-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="21aa3-128">configManager</span><span class="sxs-lookup"><span data-stu-id="21aa3-128">configManager</span></span>|<span data-ttu-id="21aa3-129">255</span><span class="sxs-lookup"><span data-stu-id="21aa3-129">255</span></span>|<span data-ttu-id="21aa3-130">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="21aa3-130">Managed by Config Manager</span></span>|



