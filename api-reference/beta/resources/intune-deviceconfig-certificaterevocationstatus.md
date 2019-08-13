---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68f510771370e5be95a8360526d0058ff8c307b1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333704"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="9b3b8-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="9b3b8-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="9b3b8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b3b8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b3b8-106">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="9b3b8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9b3b8-107">Members</span></span>
|<span data-ttu-id="9b3b8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9b3b8-108">Member</span></span>|<span data-ttu-id="9b3b8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9b3b8-109">Value</span></span>|<span data-ttu-id="9b3b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b3b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b3b8-111">none</span><span class="sxs-lookup"><span data-stu-id="9b3b8-111">none</span></span>|<span data-ttu-id="9b3b8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9b3b8-112">0</span></span>|<span data-ttu-id="9b3b8-113">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-113">Not revoked.</span></span>|
|<span data-ttu-id="9b3b8-114">закончен</span><span class="sxs-lookup"><span data-stu-id="9b3b8-114">pending</span></span>|<span data-ttu-id="9b3b8-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9b3b8-115">1</span></span>|<span data-ttu-id="9b3b8-116">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-116">Revocation pending.</span></span>|
|<span data-ttu-id="9b3b8-117">опубликован</span><span class="sxs-lookup"><span data-stu-id="9b3b8-117">issued</span></span>|<span data-ttu-id="9b3b8-118">2</span><span class="sxs-lookup"><span data-stu-id="9b3b8-118">2</span></span>|<span data-ttu-id="9b3b8-119">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-119">Revocation command issued.</span></span>|
|<span data-ttu-id="9b3b8-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="9b3b8-120">failed</span></span>|<span data-ttu-id="9b3b8-121">4</span><span class="sxs-lookup"><span data-stu-id="9b3b8-121">3</span></span>|<span data-ttu-id="9b3b8-122">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-122">Revocation failed.</span></span>|
|<span data-ttu-id="9b3b8-123">отозван</span><span class="sxs-lookup"><span data-stu-id="9b3b8-123">revoked</span></span>|<span data-ttu-id="9b3b8-124">SP4</span><span class="sxs-lookup"><span data-stu-id="9b3b8-124">4</span></span>|<span data-ttu-id="9b3b8-125">Отозван.</span><span class="sxs-lookup"><span data-stu-id="9b3b8-125">Revoked.</span></span>|



