---
title: Тип перечисления androidDeviceOwnerAppAutoUpdatePolicyType
description: Android устройства владельцем допустимые значения состояния автоматическом устройство приложения обновите политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68dec6bb21cf27a7b5b54f9fc8a839fba3dc6f00
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419074"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="9833b-103">Тип перечисления androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="9833b-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="9833b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9833b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9833b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9833b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9833b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9833b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9833b-107">Android устройства владельцем допустимые значения состояния автоматическом устройство приложения обновите политики.</span><span class="sxs-lookup"><span data-stu-id="9833b-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="9833b-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9833b-108">Members</span></span>
|<span data-ttu-id="9833b-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9833b-109">Member</span></span>|<span data-ttu-id="9833b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9833b-110">Value</span></span>|<span data-ttu-id="9833b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9833b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9833b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9833b-112">notConfigured</span></span>|<span data-ttu-id="9833b-113">0</span><span class="sxs-lookup"><span data-stu-id="9833b-113">0</span></span>|<span data-ttu-id="9833b-114">Не настроен; Это значение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="9833b-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="9833b-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="9833b-115">userChoice</span></span>|<span data-ttu-id="9833b-116">1</span><span class="sxs-lookup"><span data-stu-id="9833b-116">1</span></span>|<span data-ttu-id="9833b-117">Пользователь может управлять автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="9833b-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="9833b-118">никогда не</span><span class="sxs-lookup"><span data-stu-id="9833b-118">never</span></span>|<span data-ttu-id="9833b-119">2</span><span class="sxs-lookup"><span data-stu-id="9833b-119">2</span></span>|<span data-ttu-id="9833b-120">Приложения никогда не auto обновляются.</span><span class="sxs-lookup"><span data-stu-id="9833b-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="9833b-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="9833b-121">wiFiOnly</span></span>|<span data-ttu-id="9833b-122">3</span><span class="sxs-lookup"><span data-stu-id="9833b-122">3</span></span>|<span data-ttu-id="9833b-123">Приложения, автоматическое обновление через Wi-Fi только.</span><span class="sxs-lookup"><span data-stu-id="9833b-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="9833b-124">всегда</span><span class="sxs-lookup"><span data-stu-id="9833b-124">always</span></span>|<span data-ttu-id="9833b-125">4</span><span class="sxs-lookup"><span data-stu-id="9833b-125">4</span></span>|<span data-ttu-id="9833b-126">Приложения, автоматически обновлены в любое время.</span><span class="sxs-lookup"><span data-stu-id="9833b-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="9833b-127">Данных может потребоваться оплата.</span><span class="sxs-lookup"><span data-stu-id="9833b-127">Data charges may apply.</span></span>|




