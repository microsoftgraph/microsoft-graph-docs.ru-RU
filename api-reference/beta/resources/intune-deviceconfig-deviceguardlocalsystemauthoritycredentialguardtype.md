---
title: Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType
description: Возможные значения параметров защиты учетных данных.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d8643744e1f5c36cf6c620ac85a6a99c9a77548
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398095"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="c8820-103">Тип перечисления deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="c8820-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="c8820-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8820-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8820-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8820-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8820-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8820-107">Возможные значения параметров защиты учетных данных.</span><span class="sxs-lookup"><span data-stu-id="c8820-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="c8820-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c8820-108">Members</span></span>
|<span data-ttu-id="c8820-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c8820-109">Member</span></span>|<span data-ttu-id="c8820-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c8820-110">Value</span></span>|<span data-ttu-id="c8820-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8820-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8820-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c8820-112">notConfigured</span></span>|<span data-ttu-id="c8820-113">0</span><span class="sxs-lookup"><span data-stu-id="c8820-113">0</span></span>|<span data-ttu-id="c8820-114">Отключает защиты учетных данных удаленно Если ранее настроили без UEFI блокировки.</span><span class="sxs-lookup"><span data-stu-id="c8820-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="c8820-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="c8820-115">enableWithUEFILock</span></span>|<span data-ttu-id="c8820-116">1</span><span class="sxs-lookup"><span data-stu-id="c8820-116">1</span></span>|<span data-ttu-id="c8820-117">Включение защиты учетных данных с UEFI блокировки.</span><span class="sxs-lookup"><span data-stu-id="c8820-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="c8820-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="c8820-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="c8820-119">2</span><span class="sxs-lookup"><span data-stu-id="c8820-119">2</span></span>|<span data-ttu-id="c8820-120">Включение защиты учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="c8820-120">Turns on Credential Guard without UEFI lock.</span></span>|




