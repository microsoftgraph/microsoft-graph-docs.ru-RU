---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330277"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="7b83b-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="7b83b-103">complianceState enum type</span></span>

> <span data-ttu-id="7b83b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b83b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b83b-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="7b83b-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="7b83b-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="7b83b-106">Members</span></span>
|<span data-ttu-id="7b83b-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="7b83b-107">Member</span></span>|<span data-ttu-id="7b83b-108">Значение</span><span class="sxs-lookup"><span data-stu-id="7b83b-108">Value</span></span>|<span data-ttu-id="7b83b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7b83b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b83b-110">unknown</span><span class="sxs-lookup"><span data-stu-id="7b83b-110">unknown</span></span>|<span data-ttu-id="7b83b-111">0</span><span class="sxs-lookup"><span data-stu-id="7b83b-111">0</span></span>|<span data-ttu-id="7b83b-112">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="7b83b-112">Unknown.</span></span>|
|<span data-ttu-id="7b83b-113">спецификации</span><span class="sxs-lookup"><span data-stu-id="7b83b-113">compliant</span></span>|<span data-ttu-id="7b83b-114">1</span><span class="sxs-lookup"><span data-stu-id="7b83b-114">1</span></span>|<span data-ttu-id="7b83b-115">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="7b83b-115">Compliant.</span></span>|
|<span data-ttu-id="7b83b-116">несовместимый</span><span class="sxs-lookup"><span data-stu-id="7b83b-116">noncompliant</span></span>|<span data-ttu-id="7b83b-117">2</span><span class="sxs-lookup"><span data-stu-id="7b83b-117">2</span></span>|<span data-ttu-id="7b83b-118">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="7b83b-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="7b83b-119">конфликта</span><span class="sxs-lookup"><span data-stu-id="7b83b-119">conflict</span></span>|<span data-ttu-id="7b83b-120">3</span><span class="sxs-lookup"><span data-stu-id="7b83b-120">3</span></span>|<span data-ttu-id="7b83b-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="7b83b-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="7b83b-122">error</span><span class="sxs-lookup"><span data-stu-id="7b83b-122">error</span></span>|<span data-ttu-id="7b83b-123">4</span><span class="sxs-lookup"><span data-stu-id="7b83b-123">4</span></span>|<span data-ttu-id="7b83b-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="7b83b-124">Error.</span></span>|
|<span data-ttu-id="7b83b-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="7b83b-125">inGracePeriod</span></span>|<span data-ttu-id="7b83b-126">254</span><span class="sxs-lookup"><span data-stu-id="7b83b-126">254</span></span>|<span data-ttu-id="7b83b-127">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="7b83b-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="7b83b-128">configManager</span><span class="sxs-lookup"><span data-stu-id="7b83b-128">configManager</span></span>|<span data-ttu-id="7b83b-129">255</span><span class="sxs-lookup"><span data-stu-id="7b83b-129">255</span></span>|<span data-ttu-id="7b83b-130">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="7b83b-130">Managed by Config Manager</span></span>|



