---
title: тип перечисления deviceComplianceActionType
description: ПереЧисление типов запланированных действий
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d824f579787bf24cc56704a1c8a9df280d969809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173509"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="9460a-103">тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9460a-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="9460a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9460a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9460a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9460a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9460a-106">ПереЧисление типов запланированных действий</span><span class="sxs-lookup"><span data-stu-id="9460a-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="9460a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9460a-107">Members</span></span>
|<span data-ttu-id="9460a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9460a-108">Member</span></span>|<span data-ttu-id="9460a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9460a-109">Value</span></span>|<span data-ttu-id="9460a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9460a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9460a-111">noAction</span><span class="sxs-lookup"><span data-stu-id="9460a-111">noAction</span></span>|<span data-ttu-id="9460a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9460a-112">0</span></span>|<span data-ttu-id="9460a-113">Без действий</span><span class="sxs-lookup"><span data-stu-id="9460a-113">No Action</span></span>|
|<span data-ttu-id="9460a-114">уведомляющее</span><span class="sxs-lookup"><span data-stu-id="9460a-114">notification</span></span>|<span data-ttu-id="9460a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9460a-115">1</span></span>|<span data-ttu-id="9460a-116">Уведомление об отПравке</span><span class="sxs-lookup"><span data-stu-id="9460a-116">Send Notification</span></span>|
|<span data-ttu-id="9460a-117">блок</span><span class="sxs-lookup"><span data-stu-id="9460a-117">block</span></span>|<span data-ttu-id="9460a-118">2</span><span class="sxs-lookup"><span data-stu-id="9460a-118">2</span></span>|<span data-ttu-id="9460a-119">Блокировка устройства в AAD</span><span class="sxs-lookup"><span data-stu-id="9460a-119">Block the device in AAD</span></span>|
|<span data-ttu-id="9460a-120">снять</span><span class="sxs-lookup"><span data-stu-id="9460a-120">retire</span></span>|<span data-ttu-id="9460a-121">4</span><span class="sxs-lookup"><span data-stu-id="9460a-121">3</span></span>|<span data-ttu-id="9460a-122">Прекращение использования устройства</span><span class="sxs-lookup"><span data-stu-id="9460a-122">Retire the device</span></span>|
|<span data-ttu-id="9460a-123">Очистка</span><span class="sxs-lookup"><span data-stu-id="9460a-123">wipe</span></span>|<span data-ttu-id="9460a-124">4</span><span class="sxs-lookup"><span data-stu-id="9460a-124">4</span></span>|<span data-ttu-id="9460a-125">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="9460a-125">Wipe the device</span></span>|
|<span data-ttu-id="9460a-126">Ремовересаурцеакцесспрофилес</span><span class="sxs-lookup"><span data-stu-id="9460a-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="9460a-127">17:00</span><span class="sxs-lookup"><span data-stu-id="9460a-127">5</span></span>|<span data-ttu-id="9460a-128">Удаление профилей доступа к ресурсам с устройства</span><span class="sxs-lookup"><span data-stu-id="9460a-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="9460a-129">Пушнотификатион</span><span class="sxs-lookup"><span data-stu-id="9460a-129">pushNotification</span></span>|<span data-ttu-id="9460a-130">10</span><span class="sxs-lookup"><span data-stu-id="9460a-130">9</span></span>|<span data-ttu-id="9460a-131">Отправка push-уведомления на устройство</span><span class="sxs-lookup"><span data-stu-id="9460a-131">Send push notification to device</span></span>|
|<span data-ttu-id="9460a-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="9460a-132">remoteLock</span></span>|<span data-ttu-id="9460a-133">десяти</span><span class="sxs-lookup"><span data-stu-id="9460a-133">10</span></span>|<span data-ttu-id="9460a-134">Удаленная блокировка устройства</span><span class="sxs-lookup"><span data-stu-id="9460a-134">Remotely lock the device</span></span>|




