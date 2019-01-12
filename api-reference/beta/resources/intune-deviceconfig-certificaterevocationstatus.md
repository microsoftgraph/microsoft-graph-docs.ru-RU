---
title: Тип перечисления certificateRevocationStatus
description: Сертификат отозван.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1c77e267da5528088a7a8ef6400a872790aaf3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983123"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="4cebc-103">Тип перечисления certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="4cebc-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="4cebc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4cebc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cebc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cebc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cebc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4cebc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cebc-107">Сертификат отозван.</span><span class="sxs-lookup"><span data-stu-id="4cebc-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="4cebc-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4cebc-108">Members</span></span>
|<span data-ttu-id="4cebc-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4cebc-109">Member</span></span>|<span data-ttu-id="4cebc-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4cebc-110">Value</span></span>|<span data-ttu-id="4cebc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4cebc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cebc-112">Нет</span><span class="sxs-lookup"><span data-stu-id="4cebc-112">none</span></span>|<span data-ttu-id="4cebc-113">0</span><span class="sxs-lookup"><span data-stu-id="4cebc-113">0</span></span>|<span data-ttu-id="4cebc-114">Не был отозван.</span><span class="sxs-lookup"><span data-stu-id="4cebc-114">Not revoked.</span></span>|
|<span data-ttu-id="4cebc-115">Ожидание</span><span class="sxs-lookup"><span data-stu-id="4cebc-115">pending</span></span>|<span data-ttu-id="4cebc-116">1</span><span class="sxs-lookup"><span data-stu-id="4cebc-116">1</span></span>|<span data-ttu-id="4cebc-117">Отзыва ожидающие.</span><span class="sxs-lookup"><span data-stu-id="4cebc-117">Revocation pending.</span></span>|
|<span data-ttu-id="4cebc-118">выдан</span><span class="sxs-lookup"><span data-stu-id="4cebc-118">issued</span></span>|<span data-ttu-id="4cebc-119">2</span><span class="sxs-lookup"><span data-stu-id="4cebc-119">2</span></span>|<span data-ttu-id="4cebc-120">Отзыва команды.</span><span class="sxs-lookup"><span data-stu-id="4cebc-120">Revocation command issued.</span></span>|
|<span data-ttu-id="4cebc-121">failed</span><span class="sxs-lookup"><span data-stu-id="4cebc-121">failed</span></span>|<span data-ttu-id="4cebc-122">3</span><span class="sxs-lookup"><span data-stu-id="4cebc-122">3</span></span>|<span data-ttu-id="4cebc-123">Не удалось отзыва.</span><span class="sxs-lookup"><span data-stu-id="4cebc-123">Revocation failed.</span></span>|
|<span data-ttu-id="4cebc-124">отменено</span><span class="sxs-lookup"><span data-stu-id="4cebc-124">revoked</span></span>|<span data-ttu-id="4cebc-125">4</span><span class="sxs-lookup"><span data-stu-id="4cebc-125">4</span></span>|<span data-ttu-id="4cebc-126">Был отозван.</span><span class="sxs-lookup"><span data-stu-id="4cebc-126">Revoked.</span></span>|





