---
title: Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров защиты учетных данных.
author: tfitzmac
ms.openlocfilehash: 6f6c952d1c480d42db45de6345eba883ff5848a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346965"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="4d2f2-103">Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="4d2f2-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="4d2f2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d2f2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d2f2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d2f2-107">Возможные значения параметров защиты учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="4d2f2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4d2f2-108">Members</span></span>
|<span data-ttu-id="4d2f2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4d2f2-109">Member</span></span>|<span data-ttu-id="4d2f2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4d2f2-110">Value</span></span>|<span data-ttu-id="4d2f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d2f2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4d2f2-112">notConfigured</span></span>|<span data-ttu-id="4d2f2-113">0</span><span class="sxs-lookup"><span data-stu-id="4d2f2-113">0</span></span>|<span data-ttu-id="4d2f2-114">Отключает защиты учетных данных удаленно Если ранее настроили без UEFI блокировки.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="4d2f2-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="4d2f2-115">enableWithUEFILock</span></span>|<span data-ttu-id="4d2f2-116">1</span><span class="sxs-lookup"><span data-stu-id="4d2f2-116">1</span></span>|<span data-ttu-id="4d2f2-117">Включение защиты учетных данных с UEFI блокировки.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="4d2f2-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="4d2f2-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="4d2f2-119">2</span><span class="sxs-lookup"><span data-stu-id="4d2f2-119">2</span></span>|<span data-ttu-id="4d2f2-120">Включение защиты учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="4d2f2-120">Turns on Credential Guard without UEFI lock.</span></span>|





