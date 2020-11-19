---
title: тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе
description: Возможные значения параметров Credential Guard.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8467f60fba373265695a44533a25461e8d890824
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216131"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="1d7a2-103">тип перечисления Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="1d7a2-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="1d7a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d7a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d7a2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d7a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d7a2-107">Возможные значения параметров Credential Guard.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="1d7a2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1d7a2-108">Members</span></span>
|<span data-ttu-id="1d7a2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d7a2-109">Member</span></span>|<span data-ttu-id="1d7a2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1d7a2-110">Value</span></span>|<span data-ttu-id="1d7a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d7a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d7a2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1d7a2-112">notConfigured</span></span>|<span data-ttu-id="1d7a2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1d7a2-113">0</span></span>|<span data-ttu-id="1d7a2-114">Отключает Credential Guard удаленно, если ранее настроено без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="1d7a2-115">енаблевисуефилокк</span><span class="sxs-lookup"><span data-stu-id="1d7a2-115">enableWithUEFILock</span></span>|<span data-ttu-id="1d7a2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="1d7a2-116">1</span></span>|<span data-ttu-id="1d7a2-117">Включает защиту учетных данных с блокировкой UEFI.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="1d7a2-118">енаблевисаутуефилокк</span><span class="sxs-lookup"><span data-stu-id="1d7a2-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="1d7a2-119">2</span><span class="sxs-lookup"><span data-stu-id="1d7a2-119">2</span></span>|<span data-ttu-id="1d7a2-120">Включает защиту учетных данных без блокировки UEFI.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="1d7a2-121">отключение</span><span class="sxs-lookup"><span data-stu-id="1d7a2-121">disable</span></span>|<span data-ttu-id="1d7a2-122">4</span><span class="sxs-lookup"><span data-stu-id="1d7a2-122">3</span></span>|<span data-ttu-id="1d7a2-123">Отключает защиту учетных данных.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-123">Disables Credential Guard.</span></span> <span data-ttu-id="1d7a2-124">Это значение ОС по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1d7a2-124">This is the default OS value.</span></span>|




