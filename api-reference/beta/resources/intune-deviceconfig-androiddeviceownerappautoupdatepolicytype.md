---
title: Тип перечисления androidDeviceOwnerAppAutoUpdatePolicyType
description: Android устройства владельцем допустимые значения состояния автоматическом устройство приложения обновите политики.
ms.openlocfilehash: 0287a26b4974bc0b376341ca91791d1fa768a9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074817"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="c0388-103">Тип перечисления androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="c0388-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="c0388-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0388-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0388-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0388-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0388-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0388-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0388-107">Android устройства владельцем допустимые значения состояния автоматическом устройство приложения обновите политики.</span><span class="sxs-lookup"><span data-stu-id="c0388-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="c0388-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c0388-108">Members</span></span>
|<span data-ttu-id="c0388-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c0388-109">Member</span></span>|<span data-ttu-id="c0388-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c0388-110">Value</span></span>|<span data-ttu-id="c0388-111">Description</span><span class="sxs-lookup"><span data-stu-id="c0388-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0388-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c0388-112">notConfigured</span></span>|<span data-ttu-id="c0388-113">0</span><span class="sxs-lookup"><span data-stu-id="c0388-113">0</span></span>|<span data-ttu-id="c0388-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="c0388-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="c0388-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="c0388-115">userChoice</span></span>|<span data-ttu-id="c0388-116">1</span><span class="sxs-lookup"><span data-stu-id="c0388-116">1</span></span>|<span data-ttu-id="c0388-117">Пользователь может управлять автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="c0388-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="c0388-118">никогда не</span><span class="sxs-lookup"><span data-stu-id="c0388-118">never</span></span>|<span data-ttu-id="c0388-119">2</span><span class="sxs-lookup"><span data-stu-id="c0388-119">2</span></span>|<span data-ttu-id="c0388-120">Приложения никогда не auto обновляются.</span><span class="sxs-lookup"><span data-stu-id="c0388-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="c0388-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="c0388-121">wiFiOnly</span></span>|<span data-ttu-id="c0388-122">3</span><span class="sxs-lookup"><span data-stu-id="c0388-122">3</span></span>|<span data-ttu-id="c0388-123">Приложения, автоматическое обновление через Wi-Fi только.</span><span class="sxs-lookup"><span data-stu-id="c0388-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="c0388-124">всегда</span><span class="sxs-lookup"><span data-stu-id="c0388-124">always</span></span>|<span data-ttu-id="c0388-125">4</span><span class="sxs-lookup"><span data-stu-id="c0388-125">4</span></span>|<span data-ttu-id="c0388-126">Приложения, автоматически обновлены в любое время.</span><span class="sxs-lookup"><span data-stu-id="c0388-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="c0388-127">Данных может потребоваться оплата.</span><span class="sxs-lookup"><span data-stu-id="c0388-127">Data charges may apply.</span></span>|





