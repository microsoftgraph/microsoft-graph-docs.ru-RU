---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940199"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="8e504-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="8e504-103">complianceState enum type</span></span>

> <span data-ttu-id="8e504-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e504-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e504-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="8e504-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="8e504-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="8e504-106">Members</span></span>
|<span data-ttu-id="8e504-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="8e504-107">Member</span></span>|<span data-ttu-id="8e504-108">Значение</span><span class="sxs-lookup"><span data-stu-id="8e504-108">Value</span></span>|<span data-ttu-id="8e504-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8e504-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e504-110">unknown</span><span class="sxs-lookup"><span data-stu-id="8e504-110">unknown</span></span>|<span data-ttu-id="8e504-111">0</span><span class="sxs-lookup"><span data-stu-id="8e504-111">0</span></span>|<span data-ttu-id="8e504-112">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="8e504-112">Unknown.</span></span>|
|<span data-ttu-id="8e504-113">спецификации</span><span class="sxs-lookup"><span data-stu-id="8e504-113">compliant</span></span>|<span data-ttu-id="8e504-114">1</span><span class="sxs-lookup"><span data-stu-id="8e504-114">1</span></span>|<span data-ttu-id="8e504-115">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="8e504-115">Compliant.</span></span>|
|<span data-ttu-id="8e504-116">несовместимый</span><span class="sxs-lookup"><span data-stu-id="8e504-116">noncompliant</span></span>|<span data-ttu-id="8e504-117">2</span><span class="sxs-lookup"><span data-stu-id="8e504-117">2</span></span>|<span data-ttu-id="8e504-118">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="8e504-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="8e504-119">конфликта</span><span class="sxs-lookup"><span data-stu-id="8e504-119">conflict</span></span>|<span data-ttu-id="8e504-120">3</span><span class="sxs-lookup"><span data-stu-id="8e504-120">3</span></span>|<span data-ttu-id="8e504-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="8e504-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="8e504-122">error</span><span class="sxs-lookup"><span data-stu-id="8e504-122">error</span></span>|<span data-ttu-id="8e504-123">4</span><span class="sxs-lookup"><span data-stu-id="8e504-123">4</span></span>|<span data-ttu-id="8e504-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="8e504-124">Error.</span></span>|
|<span data-ttu-id="8e504-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="8e504-125">inGracePeriod</span></span>|<span data-ttu-id="8e504-126">254</span><span class="sxs-lookup"><span data-stu-id="8e504-126">254</span></span>|<span data-ttu-id="8e504-127">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="8e504-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="8e504-128">configManager</span><span class="sxs-lookup"><span data-stu-id="8e504-128">configManager</span></span>|<span data-ttu-id="8e504-129">255</span><span class="sxs-lookup"><span data-stu-id="8e504-129">255</span></span>|<span data-ttu-id="8e504-130">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="8e504-130">Managed by Config Manager</span></span>|



