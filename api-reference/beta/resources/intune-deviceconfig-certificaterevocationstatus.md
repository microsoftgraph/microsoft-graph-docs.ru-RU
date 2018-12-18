---
title: Тип перечисления certificateRevocationStatus
description: Сертификат отозван.
author: tfitzmac
ms.openlocfilehash: d41845ba882136c15d944c8a7f91083e6fa47cdb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358228"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="81e27-103">Тип перечисления certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="81e27-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="81e27-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81e27-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81e27-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81e27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81e27-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81e27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81e27-107">Сертификат отозван.</span><span class="sxs-lookup"><span data-stu-id="81e27-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="81e27-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="81e27-108">Members</span></span>
|<span data-ttu-id="81e27-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="81e27-109">Member</span></span>|<span data-ttu-id="81e27-110">Значение</span><span class="sxs-lookup"><span data-stu-id="81e27-110">Value</span></span>|<span data-ttu-id="81e27-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81e27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e27-112">none</span><span class="sxs-lookup"><span data-stu-id="81e27-112">none</span></span>|<span data-ttu-id="81e27-113">0</span><span class="sxs-lookup"><span data-stu-id="81e27-113">0</span></span>|<span data-ttu-id="81e27-114">Не был отозван.</span><span class="sxs-lookup"><span data-stu-id="81e27-114">Not revoked.</span></span>|
|<span data-ttu-id="81e27-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="81e27-115">pending</span></span>|<span data-ttu-id="81e27-116">1</span><span class="sxs-lookup"><span data-stu-id="81e27-116">1</span></span>|<span data-ttu-id="81e27-117">Отзыва ожидающие.</span><span class="sxs-lookup"><span data-stu-id="81e27-117">Revocation pending.</span></span>|
|<span data-ttu-id="81e27-118">выдан</span><span class="sxs-lookup"><span data-stu-id="81e27-118">issued</span></span>|<span data-ttu-id="81e27-119">2</span><span class="sxs-lookup"><span data-stu-id="81e27-119">2</span></span>|<span data-ttu-id="81e27-120">Отзыва команды.</span><span class="sxs-lookup"><span data-stu-id="81e27-120">Revocation command issued.</span></span>|
|<span data-ttu-id="81e27-121">failed</span><span class="sxs-lookup"><span data-stu-id="81e27-121">failed</span></span>|<span data-ttu-id="81e27-122">3</span><span class="sxs-lookup"><span data-stu-id="81e27-122">3</span></span>|<span data-ttu-id="81e27-123">Не удалось отзыва.</span><span class="sxs-lookup"><span data-stu-id="81e27-123">Revocation failed.</span></span>|
|<span data-ttu-id="81e27-124">отменено</span><span class="sxs-lookup"><span data-stu-id="81e27-124">revoked</span></span>|<span data-ttu-id="81e27-125">4</span><span class="sxs-lookup"><span data-stu-id="81e27-125">4</span></span>|<span data-ttu-id="81e27-126">Был отозван.</span><span class="sxs-lookup"><span data-stu-id="81e27-126">Revoked.</span></span>|





