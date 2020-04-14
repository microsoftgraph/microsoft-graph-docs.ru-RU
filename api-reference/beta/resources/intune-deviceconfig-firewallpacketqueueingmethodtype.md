---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0a6bd346c45e21c31901d7e54eda95f72fa92a23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444304"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="6b9be-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="6b9be-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="6b9be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b9be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b9be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b9be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b9be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b9be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9be-107">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="6b9be-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="6b9be-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6b9be-108">Members</span></span>
|<span data-ttu-id="6b9be-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6b9be-109">Member</span></span>|<span data-ttu-id="6b9be-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6b9be-110">Value</span></span>|<span data-ttu-id="6b9be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b9be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9be-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="6b9be-112">deviceDefault</span></span>|<span data-ttu-id="6b9be-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6b9be-113">0</span></span>|<span data-ttu-id="6b9be-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="6b9be-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="6b9be-115">отключено</span><span class="sxs-lookup"><span data-stu-id="6b9be-115">disabled</span></span>|<span data-ttu-id="6b9be-116">1,1</span><span class="sxs-lookup"><span data-stu-id="6b9be-116">1</span></span>|<span data-ttu-id="6b9be-117">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="6b9be-117">Disable packet queuing</span></span>|
|<span data-ttu-id="6b9be-118">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="6b9be-118">queueInbound</span></span>|<span data-ttu-id="6b9be-119">2</span><span class="sxs-lookup"><span data-stu-id="6b9be-119">2</span></span>|<span data-ttu-id="6b9be-120">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="6b9be-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="6b9be-121">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="6b9be-121">queueOutbound</span></span>|<span data-ttu-id="6b9be-122">4</span><span class="sxs-lookup"><span data-stu-id="6b9be-122">3</span></span>|<span data-ttu-id="6b9be-123">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="6b9be-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="6b9be-124">куеуебос</span><span class="sxs-lookup"><span data-stu-id="6b9be-124">queueBoth</span></span>|<span data-ttu-id="6b9be-125">4 </span><span class="sxs-lookup"><span data-stu-id="6b9be-125">4</span></span>|<span data-ttu-id="6b9be-126">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="6b9be-126">Queue both inbound and outbound packets</span></span>|



