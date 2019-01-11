---
title: Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров защиты учетных данных.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7f59fed69647ead4ccdda0523ae80571aebcb57c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871584"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="ba9b7-103">Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="ba9b7-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="ba9b7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba9b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba9b7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba9b7-107">Возможные значения параметров защиты учетных данных.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="ba9b7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ba9b7-108">Members</span></span>
|<span data-ttu-id="ba9b7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ba9b7-109">Member</span></span>|<span data-ttu-id="ba9b7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ba9b7-110">Value</span></span>|<span data-ttu-id="ba9b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba9b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba9b7-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ba9b7-112">notConfigured</span></span>|<span data-ttu-id="ba9b7-113">0</span><span class="sxs-lookup"><span data-stu-id="ba9b7-113">0</span></span>|<span data-ttu-id="ba9b7-114">Отключает защиты учетных данных удаленно Если ранее настроили без UEFI блокировки.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="ba9b7-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="ba9b7-115">enableWithUEFILock</span></span>|<span data-ttu-id="ba9b7-116">1</span><span class="sxs-lookup"><span data-stu-id="ba9b7-116">1</span></span>|<span data-ttu-id="ba9b7-117">Включение защиты учетных данных с UEFI блокировки.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="ba9b7-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="ba9b7-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="ba9b7-119">2</span><span class="sxs-lookup"><span data-stu-id="ba9b7-119">2</span></span>|<span data-ttu-id="ba9b7-120">Включение защиты учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="ba9b7-120">Turns on Credential Guard without UEFI lock.</span></span>|





