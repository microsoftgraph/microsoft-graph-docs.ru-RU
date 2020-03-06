---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b5976d7ff06620db9958dacdfdd0b8b0c81a191
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530728"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="3ef5c-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="3ef5c-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="3ef5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ef5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ef5c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ef5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ef5c-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="3ef5c-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="3ef5c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3ef5c-107">Members</span></span>
|<span data-ttu-id="3ef5c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3ef5c-108">Member</span></span>|<span data-ttu-id="3ef5c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3ef5c-109">Value</span></span>|<span data-ttu-id="3ef5c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef5c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ef5c-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="3ef5c-111">deviceDefault</span></span>|<span data-ttu-id="3ef5c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3ef5c-112">0</span></span>|<span data-ttu-id="3ef5c-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="3ef5c-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="3ef5c-114">активирован</span><span class="sxs-lookup"><span data-stu-id="3ef5c-114">disabled</span></span>|<span data-ttu-id="3ef5c-115">1 </span><span class="sxs-lookup"><span data-stu-id="3ef5c-115">1</span></span>|<span data-ttu-id="3ef5c-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="3ef5c-116">Disable packet queuing</span></span>|
|<span data-ttu-id="3ef5c-117">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="3ef5c-117">queueInbound</span></span>|<span data-ttu-id="3ef5c-118">2 </span><span class="sxs-lookup"><span data-stu-id="3ef5c-118">2</span></span>|<span data-ttu-id="3ef5c-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="3ef5c-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="3ef5c-120">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="3ef5c-120">queueOutbound</span></span>|<span data-ttu-id="3ef5c-121">3 </span><span class="sxs-lookup"><span data-stu-id="3ef5c-121">3</span></span>|<span data-ttu-id="3ef5c-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="3ef5c-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="3ef5c-123">куеуебос</span><span class="sxs-lookup"><span data-stu-id="3ef5c-123">queueBoth</span></span>|<span data-ttu-id="3ef5c-124">4 </span><span class="sxs-lookup"><span data-stu-id="3ef5c-124">4</span></span>|<span data-ttu-id="3ef5c-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="3ef5c-125">Queue both inbound and outbound packets</span></span>|




