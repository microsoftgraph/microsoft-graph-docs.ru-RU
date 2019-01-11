---
title: Тип перечисления certificateRevocationStatus
description: Сертификат отозван.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d24d515f992ed396c3530595240a107852d83e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868308"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="15af9-103">Тип перечисления certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="15af9-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="15af9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15af9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15af9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15af9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15af9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15af9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15af9-107">Сертификат отозван.</span><span class="sxs-lookup"><span data-stu-id="15af9-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="15af9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="15af9-108">Members</span></span>
|<span data-ttu-id="15af9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="15af9-109">Member</span></span>|<span data-ttu-id="15af9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="15af9-110">Value</span></span>|<span data-ttu-id="15af9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15af9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15af9-112">Нет</span><span class="sxs-lookup"><span data-stu-id="15af9-112">none</span></span>|<span data-ttu-id="15af9-113">0</span><span class="sxs-lookup"><span data-stu-id="15af9-113">0</span></span>|<span data-ttu-id="15af9-114">Не был отозван.</span><span class="sxs-lookup"><span data-stu-id="15af9-114">Not revoked.</span></span>|
|<span data-ttu-id="15af9-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="15af9-115">pending</span></span>|<span data-ttu-id="15af9-116">1</span><span class="sxs-lookup"><span data-stu-id="15af9-116">1</span></span>|<span data-ttu-id="15af9-117">Отзыва ожидающие.</span><span class="sxs-lookup"><span data-stu-id="15af9-117">Revocation pending.</span></span>|
|<span data-ttu-id="15af9-118">выдан</span><span class="sxs-lookup"><span data-stu-id="15af9-118">issued</span></span>|<span data-ttu-id="15af9-119">2</span><span class="sxs-lookup"><span data-stu-id="15af9-119">2</span></span>|<span data-ttu-id="15af9-120">Отзыва команды.</span><span class="sxs-lookup"><span data-stu-id="15af9-120">Revocation command issued.</span></span>|
|<span data-ttu-id="15af9-121">failed</span><span class="sxs-lookup"><span data-stu-id="15af9-121">failed</span></span>|<span data-ttu-id="15af9-122">3</span><span class="sxs-lookup"><span data-stu-id="15af9-122">3</span></span>|<span data-ttu-id="15af9-123">Не удалось отзыва.</span><span class="sxs-lookup"><span data-stu-id="15af9-123">Revocation failed.</span></span>|
|<span data-ttu-id="15af9-124">отменено</span><span class="sxs-lookup"><span data-stu-id="15af9-124">revoked</span></span>|<span data-ttu-id="15af9-125">4</span><span class="sxs-lookup"><span data-stu-id="15af9-125">4</span></span>|<span data-ttu-id="15af9-126">Был отозван.</span><span class="sxs-lookup"><span data-stu-id="15af9-126">Revoked.</span></span>|





