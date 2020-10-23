---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4616a562bc6cedda543c564660557cb9e67d7dc4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730646"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="5e5c2-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="5e5c2-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="5e5c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e5c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e5c2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e5c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e5c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e5c2-107">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="5e5c2-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="5e5c2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="5e5c2-108">Members</span></span>
|<span data-ttu-id="5e5c2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="5e5c2-109">Member</span></span>|<span data-ttu-id="5e5c2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="5e5c2-110">Value</span></span>|<span data-ttu-id="5e5c2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e5c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e5c2-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="5e5c2-112">deviceDefault</span></span>|<span data-ttu-id="5e5c2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="5e5c2-113">0</span></span>|<span data-ttu-id="5e5c2-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="5e5c2-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="5e5c2-115">отключено</span><span class="sxs-lookup"><span data-stu-id="5e5c2-115">disabled</span></span>|<span data-ttu-id="5e5c2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="5e5c2-116">1</span></span>|<span data-ttu-id="5e5c2-117">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="5e5c2-117">Disable packet queuing</span></span>|
|<span data-ttu-id="5e5c2-118">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="5e5c2-118">queueInbound</span></span>|<span data-ttu-id="5e5c2-119">2</span><span class="sxs-lookup"><span data-stu-id="5e5c2-119">2</span></span>|<span data-ttu-id="5e5c2-120">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="5e5c2-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="5e5c2-121">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="5e5c2-121">queueOutbound</span></span>|<span data-ttu-id="5e5c2-122">4</span><span class="sxs-lookup"><span data-stu-id="5e5c2-122">3</span></span>|<span data-ttu-id="5e5c2-123">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="5e5c2-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="5e5c2-124">куеуебос</span><span class="sxs-lookup"><span data-stu-id="5e5c2-124">queueBoth</span></span>|<span data-ttu-id="5e5c2-125">4 </span><span class="sxs-lookup"><span data-stu-id="5e5c2-125">4</span></span>|<span data-ttu-id="5e5c2-126">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="5e5c2-126">Queue both inbound and outbound packets</span></span>|





