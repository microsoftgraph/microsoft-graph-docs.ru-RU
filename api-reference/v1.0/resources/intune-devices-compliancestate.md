---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53b17f258f577e0842dbfc81c6341303f6b43799
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820344"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="dcce0-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="dcce0-103">complianceState enum type</span></span>

> <span data-ttu-id="dcce0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dcce0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dcce0-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="dcce0-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="dcce0-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="dcce0-106">Members</span></span>
|<span data-ttu-id="dcce0-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="dcce0-107">Member</span></span>|<span data-ttu-id="dcce0-108">Значение</span><span class="sxs-lookup"><span data-stu-id="dcce0-108">Value</span></span>|<span data-ttu-id="dcce0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dcce0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcce0-110">unknown</span><span class="sxs-lookup"><span data-stu-id="dcce0-110">unknown</span></span>|<span data-ttu-id="dcce0-111">0</span><span class="sxs-lookup"><span data-stu-id="dcce0-111">0</span></span>|<span data-ttu-id="dcce0-112">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="dcce0-112">Unknown.</span></span>|
|<span data-ttu-id="dcce0-113">спецификации</span><span class="sxs-lookup"><span data-stu-id="dcce0-113">compliant</span></span>|<span data-ttu-id="dcce0-114">1</span><span class="sxs-lookup"><span data-stu-id="dcce0-114">1</span></span>|<span data-ttu-id="dcce0-115">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="dcce0-115">Compliant.</span></span>|
|<span data-ttu-id="dcce0-116">несовместимый</span><span class="sxs-lookup"><span data-stu-id="dcce0-116">noncompliant</span></span>|<span data-ttu-id="dcce0-117">2</span><span class="sxs-lookup"><span data-stu-id="dcce0-117">2</span></span>|<span data-ttu-id="dcce0-118">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="dcce0-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="dcce0-119">конфликта</span><span class="sxs-lookup"><span data-stu-id="dcce0-119">conflict</span></span>|<span data-ttu-id="dcce0-120">3</span><span class="sxs-lookup"><span data-stu-id="dcce0-120">3</span></span>|<span data-ttu-id="dcce0-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="dcce0-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="dcce0-122">error</span><span class="sxs-lookup"><span data-stu-id="dcce0-122">error</span></span>|<span data-ttu-id="dcce0-123">4</span><span class="sxs-lookup"><span data-stu-id="dcce0-123">4</span></span>|<span data-ttu-id="dcce0-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="dcce0-124">Error.</span></span>|
|<span data-ttu-id="dcce0-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="dcce0-125">inGracePeriod</span></span>|<span data-ttu-id="dcce0-126">254</span><span class="sxs-lookup"><span data-stu-id="dcce0-126">254</span></span>|<span data-ttu-id="dcce0-127">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="dcce0-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="dcce0-128">configManager</span><span class="sxs-lookup"><span data-stu-id="dcce0-128">configManager</span></span>|<span data-ttu-id="dcce0-129">255</span><span class="sxs-lookup"><span data-stu-id="dcce0-129">255</span></span>|<span data-ttu-id="dcce0-130">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="dcce0-130">Managed by Config Manager</span></span>|



