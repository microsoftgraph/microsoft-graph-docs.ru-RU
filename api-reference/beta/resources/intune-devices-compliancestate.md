---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8936d2116a3aaa8e77905174b46a3997c317cfda
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968717"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="0a4d9-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="0a4d9-103">complianceState enum type</span></span>

> <span data-ttu-id="0a4d9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a4d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a4d9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a4d9-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="0a4d9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0a4d9-108">Members</span></span>
|<span data-ttu-id="0a4d9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0a4d9-109">Member</span></span>|<span data-ttu-id="0a4d9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0a4d9-110">Value</span></span>|<span data-ttu-id="0a4d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a4d9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="0a4d9-112">unknown</span></span>|<span data-ttu-id="0a4d9-113">0</span><span class="sxs-lookup"><span data-stu-id="0a4d9-113">0</span></span>|<span data-ttu-id="0a4d9-114">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-114">Unknown.</span></span>|
|<span data-ttu-id="0a4d9-115">спецификации</span><span class="sxs-lookup"><span data-stu-id="0a4d9-115">compliant</span></span>|<span data-ttu-id="0a4d9-116">1</span><span class="sxs-lookup"><span data-stu-id="0a4d9-116">1</span></span>|<span data-ttu-id="0a4d9-117">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-117">Compliant.</span></span>|
|<span data-ttu-id="0a4d9-118">несовместимый</span><span class="sxs-lookup"><span data-stu-id="0a4d9-118">noncompliant</span></span>|<span data-ttu-id="0a4d9-119">2</span><span class="sxs-lookup"><span data-stu-id="0a4d9-119">2</span></span>|<span data-ttu-id="0a4d9-120">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="0a4d9-121">конфликта</span><span class="sxs-lookup"><span data-stu-id="0a4d9-121">conflict</span></span>|<span data-ttu-id="0a4d9-122">3</span><span class="sxs-lookup"><span data-stu-id="0a4d9-122">3</span></span>|<span data-ttu-id="0a4d9-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="0a4d9-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="0a4d9-124">error</span><span class="sxs-lookup"><span data-stu-id="0a4d9-124">error</span></span>|<span data-ttu-id="0a4d9-125">4</span><span class="sxs-lookup"><span data-stu-id="0a4d9-125">4</span></span>|<span data-ttu-id="0a4d9-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="0a4d9-126">Error.</span></span>|
|<span data-ttu-id="0a4d9-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="0a4d9-127">inGracePeriod</span></span>|<span data-ttu-id="0a4d9-128">254</span><span class="sxs-lookup"><span data-stu-id="0a4d9-128">254</span></span>|<span data-ttu-id="0a4d9-129">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="0a4d9-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="0a4d9-130">configManager</span><span class="sxs-lookup"><span data-stu-id="0a4d9-130">configManager</span></span>|<span data-ttu-id="0a4d9-131">255</span><span class="sxs-lookup"><span data-stu-id="0a4d9-131">255</span></span>|<span data-ttu-id="0a4d9-132">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="0a4d9-132">Managed by Config Manager</span></span>|





