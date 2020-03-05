---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b134e00e0237e407331f0ea0554c54dcf0d39ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529989"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="15aed-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="15aed-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="15aed-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15aed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15aed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15aed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15aed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15aed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15aed-107">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="15aed-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="15aed-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="15aed-108">Members</span></span>
|<span data-ttu-id="15aed-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="15aed-109">Member</span></span>|<span data-ttu-id="15aed-110">Значение</span><span class="sxs-lookup"><span data-stu-id="15aed-110">Value</span></span>|<span data-ttu-id="15aed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15aed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15aed-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="15aed-112">deviceDefault</span></span>|<span data-ttu-id="15aed-113">нуль</span><span class="sxs-lookup"><span data-stu-id="15aed-113">0</span></span>|<span data-ttu-id="15aed-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="15aed-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="15aed-115">активирован</span><span class="sxs-lookup"><span data-stu-id="15aed-115">disabled</span></span>|<span data-ttu-id="15aed-116">1 </span><span class="sxs-lookup"><span data-stu-id="15aed-116">1</span></span>|<span data-ttu-id="15aed-117">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="15aed-117">Disable packet queuing</span></span>|
|<span data-ttu-id="15aed-118">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="15aed-118">queueInbound</span></span>|<span data-ttu-id="15aed-119">2 </span><span class="sxs-lookup"><span data-stu-id="15aed-119">2</span></span>|<span data-ttu-id="15aed-120">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="15aed-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="15aed-121">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="15aed-121">queueOutbound</span></span>|<span data-ttu-id="15aed-122">3 </span><span class="sxs-lookup"><span data-stu-id="15aed-122">3</span></span>|<span data-ttu-id="15aed-123">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="15aed-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="15aed-124">куеуебос</span><span class="sxs-lookup"><span data-stu-id="15aed-124">queueBoth</span></span>|<span data-ttu-id="15aed-125">4 </span><span class="sxs-lookup"><span data-stu-id="15aed-125">4</span></span>|<span data-ttu-id="15aed-126">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="15aed-126">Queue both inbound and outbound packets</span></span>|



