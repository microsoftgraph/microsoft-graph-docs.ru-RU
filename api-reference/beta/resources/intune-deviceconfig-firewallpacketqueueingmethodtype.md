---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 52765eedfc7df894be32184a7a5f071ae27552cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001322"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="7ea77-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="7ea77-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="7ea77-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ea77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ea77-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ea77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ea77-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="7ea77-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="7ea77-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7ea77-107">Members</span></span>
|<span data-ttu-id="7ea77-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7ea77-108">Member</span></span>|<span data-ttu-id="7ea77-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7ea77-109">Value</span></span>|<span data-ttu-id="7ea77-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ea77-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ea77-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="7ea77-111">deviceDefault</span></span>|<span data-ttu-id="7ea77-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7ea77-112">0</span></span>|<span data-ttu-id="7ea77-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="7ea77-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7ea77-114">активирован</span><span class="sxs-lookup"><span data-stu-id="7ea77-114">disabled</span></span>|<span data-ttu-id="7ea77-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7ea77-115">1</span></span>|<span data-ttu-id="7ea77-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="7ea77-116">Disable packet queuing</span></span>|
|<span data-ttu-id="7ea77-117">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="7ea77-117">queueInbound</span></span>|<span data-ttu-id="7ea77-118">2</span><span class="sxs-lookup"><span data-stu-id="7ea77-118">2</span></span>|<span data-ttu-id="7ea77-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="7ea77-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="7ea77-120">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="7ea77-120">queueOutbound</span></span>|<span data-ttu-id="7ea77-121">4</span><span class="sxs-lookup"><span data-stu-id="7ea77-121">3</span></span>|<span data-ttu-id="7ea77-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="7ea77-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="7ea77-123">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="7ea77-123">queueBoth</span></span>|<span data-ttu-id="7ea77-124">SP4</span><span class="sxs-lookup"><span data-stu-id="7ea77-124">4</span></span>|<span data-ttu-id="7ea77-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="7ea77-125">Queue both inbound and outbound packets</span></span>|





