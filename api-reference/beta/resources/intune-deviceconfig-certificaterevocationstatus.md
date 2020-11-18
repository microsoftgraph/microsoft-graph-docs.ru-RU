---
title: тип перечисления Цертификатеревокатионстатус
description: Состояние отзыва сертификата.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 89f0ce18f1f2d81373ac43497b6d3e55344b5a18
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199618"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="9cf59-103">тип перечисления Цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="9cf59-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="9cf59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cf59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cf59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cf59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf59-107">Состояние отзыва сертификата.</span><span class="sxs-lookup"><span data-stu-id="9cf59-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="9cf59-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9cf59-108">Members</span></span>
|<span data-ttu-id="9cf59-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9cf59-109">Member</span></span>|<span data-ttu-id="9cf59-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9cf59-110">Value</span></span>|<span data-ttu-id="9cf59-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9cf59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf59-112">Нет</span><span class="sxs-lookup"><span data-stu-id="9cf59-112">none</span></span>|<span data-ttu-id="9cf59-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9cf59-113">0</span></span>|<span data-ttu-id="9cf59-114">Не отозван.</span><span class="sxs-lookup"><span data-stu-id="9cf59-114">Not revoked.</span></span>|
|<span data-ttu-id="9cf59-115">закончен</span><span class="sxs-lookup"><span data-stu-id="9cf59-115">pending</span></span>|<span data-ttu-id="9cf59-116">1,1</span><span class="sxs-lookup"><span data-stu-id="9cf59-116">1</span></span>|<span data-ttu-id="9cf59-117">Отзыв ожидается.</span><span class="sxs-lookup"><span data-stu-id="9cf59-117">Revocation pending.</span></span>|
|<span data-ttu-id="9cf59-118">опубликован</span><span class="sxs-lookup"><span data-stu-id="9cf59-118">issued</span></span>|<span data-ttu-id="9cf59-119">2</span><span class="sxs-lookup"><span data-stu-id="9cf59-119">2</span></span>|<span data-ttu-id="9cf59-120">Выдана команда отзыва.</span><span class="sxs-lookup"><span data-stu-id="9cf59-120">Revocation command issued.</span></span>|
|<span data-ttu-id="9cf59-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="9cf59-121">failed</span></span>|<span data-ttu-id="9cf59-122">4</span><span class="sxs-lookup"><span data-stu-id="9cf59-122">3</span></span>|<span data-ttu-id="9cf59-123">Не удалось выполнить отзыв.</span><span class="sxs-lookup"><span data-stu-id="9cf59-123">Revocation failed.</span></span>|
|<span data-ttu-id="9cf59-124">отозван</span><span class="sxs-lookup"><span data-stu-id="9cf59-124">revoked</span></span>|<span data-ttu-id="9cf59-125">4 </span><span class="sxs-lookup"><span data-stu-id="9cf59-125">4</span></span>|<span data-ttu-id="9cf59-126">Отозван.</span><span class="sxs-lookup"><span data-stu-id="9cf59-126">Revoked.</span></span>|




