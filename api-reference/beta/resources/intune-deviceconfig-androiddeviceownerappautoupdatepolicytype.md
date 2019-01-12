---
title: Тип перечисления androidDeviceOwnerAppAutoUpdatePolicyType
description: Android устройства владельцем допустимые значения состояния автоматическом устройство приложения обновите политики.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f784e951df2a9d1ee56825649da3899b0792c3a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973610"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="eccc3-103">Тип перечисления androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="eccc3-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="eccc3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eccc3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eccc3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eccc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eccc3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eccc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eccc3-107">Android устройства владельцем допустимые значения состояния автоматическом устройство приложения обновите политики.</span><span class="sxs-lookup"><span data-stu-id="eccc3-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="eccc3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="eccc3-108">Members</span></span>
|<span data-ttu-id="eccc3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="eccc3-109">Member</span></span>|<span data-ttu-id="eccc3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="eccc3-110">Value</span></span>|<span data-ttu-id="eccc3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eccc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eccc3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="eccc3-112">notConfigured</span></span>|<span data-ttu-id="eccc3-113">0</span><span class="sxs-lookup"><span data-stu-id="eccc3-113">0</span></span>|<span data-ttu-id="eccc3-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="eccc3-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="eccc3-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="eccc3-115">userChoice</span></span>|<span data-ttu-id="eccc3-116">1</span><span class="sxs-lookup"><span data-stu-id="eccc3-116">1</span></span>|<span data-ttu-id="eccc3-117">Пользователь может управлять автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="eccc3-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="eccc3-118">никогда не</span><span class="sxs-lookup"><span data-stu-id="eccc3-118">never</span></span>|<span data-ttu-id="eccc3-119">2</span><span class="sxs-lookup"><span data-stu-id="eccc3-119">2</span></span>|<span data-ttu-id="eccc3-120">Приложения никогда не auto обновляются.</span><span class="sxs-lookup"><span data-stu-id="eccc3-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="eccc3-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="eccc3-121">wiFiOnly</span></span>|<span data-ttu-id="eccc3-122">3</span><span class="sxs-lookup"><span data-stu-id="eccc3-122">3</span></span>|<span data-ttu-id="eccc3-123">Приложения, автоматическое обновление через Wi-Fi только.</span><span class="sxs-lookup"><span data-stu-id="eccc3-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="eccc3-124">всегда</span><span class="sxs-lookup"><span data-stu-id="eccc3-124">always</span></span>|<span data-ttu-id="eccc3-125">4</span><span class="sxs-lookup"><span data-stu-id="eccc3-125">4</span></span>|<span data-ttu-id="eccc3-126">Приложения, автоматически обновлены в любое время.</span><span class="sxs-lookup"><span data-stu-id="eccc3-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="eccc3-127">Данных может потребоваться оплата.</span><span class="sxs-lookup"><span data-stu-id="eccc3-127">Data charges may apply.</span></span>|





