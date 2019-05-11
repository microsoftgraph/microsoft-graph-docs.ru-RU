---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b1802e150460e1e687b8303716a723146e4ca67
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946688"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="c2b63-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="c2b63-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="c2b63-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b63-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2b63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b63-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="c2b63-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="c2b63-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c2b63-107">Members</span></span>
|<span data-ttu-id="c2b63-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c2b63-108">Member</span></span>|<span data-ttu-id="c2b63-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c2b63-109">Value</span></span>|<span data-ttu-id="c2b63-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b63-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="c2b63-111">deviceDefault</span></span>|<span data-ttu-id="c2b63-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c2b63-112">0</span></span>|<span data-ttu-id="c2b63-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="c2b63-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c2b63-114">активирован</span><span class="sxs-lookup"><span data-stu-id="c2b63-114">disabled</span></span>|<span data-ttu-id="c2b63-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c2b63-115">1</span></span>|<span data-ttu-id="c2b63-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="c2b63-116">Disable packet queuing</span></span>|
|<span data-ttu-id="c2b63-117">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="c2b63-117">queueInbound</span></span>|<span data-ttu-id="c2b63-118">2</span><span class="sxs-lookup"><span data-stu-id="c2b63-118">2</span></span>|<span data-ttu-id="c2b63-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="c2b63-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="c2b63-120">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="c2b63-120">queueOutbound</span></span>|<span data-ttu-id="c2b63-121">4</span><span class="sxs-lookup"><span data-stu-id="c2b63-121">3</span></span>|<span data-ttu-id="c2b63-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="c2b63-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="c2b63-123">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="c2b63-123">queueBoth</span></span>|<span data-ttu-id="c2b63-124">SP4</span><span class="sxs-lookup"><span data-stu-id="c2b63-124">4</span></span>|<span data-ttu-id="c2b63-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="c2b63-125">Queue both inbound and outbound packets</span></span>|




