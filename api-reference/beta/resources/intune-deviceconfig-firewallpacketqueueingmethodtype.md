---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8d4bd680061f49b91d9106f455487c72e3e7dbd7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791753"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="01ae9-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="01ae9-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="01ae9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01ae9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01ae9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01ae9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01ae9-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="01ae9-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="01ae9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="01ae9-107">Members</span></span>
|<span data-ttu-id="01ae9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="01ae9-108">Member</span></span>|<span data-ttu-id="01ae9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="01ae9-109">Value</span></span>|<span data-ttu-id="01ae9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01ae9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01ae9-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="01ae9-111">deviceDefault</span></span>|<span data-ttu-id="01ae9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="01ae9-112">0</span></span>|<span data-ttu-id="01ae9-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="01ae9-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="01ae9-114">активирован</span><span class="sxs-lookup"><span data-stu-id="01ae9-114">disabled</span></span>|<span data-ttu-id="01ae9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="01ae9-115">1</span></span>|<span data-ttu-id="01ae9-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="01ae9-116">Disable packet queuing</span></span>|
|<span data-ttu-id="01ae9-117">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="01ae9-117">queueInbound</span></span>|<span data-ttu-id="01ae9-118">2</span><span class="sxs-lookup"><span data-stu-id="01ae9-118">2</span></span>|<span data-ttu-id="01ae9-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="01ae9-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="01ae9-120">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="01ae9-120">queueOutbound</span></span>|<span data-ttu-id="01ae9-121">4</span><span class="sxs-lookup"><span data-stu-id="01ae9-121">3</span></span>|<span data-ttu-id="01ae9-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="01ae9-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="01ae9-123">куеуебос</span><span class="sxs-lookup"><span data-stu-id="01ae9-123">queueBoth</span></span>|<span data-ttu-id="01ae9-124">4 </span><span class="sxs-lookup"><span data-stu-id="01ae9-124">4</span></span>|<span data-ttu-id="01ae9-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="01ae9-125">Queue both inbound and outbound packets</span></span>|



