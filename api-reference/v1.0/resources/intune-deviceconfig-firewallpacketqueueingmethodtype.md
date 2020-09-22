---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0774a8b2fa9e2240366ef7a25edf2db252dafd4d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056704"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="d6c03-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d6c03-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="d6c03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6c03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6c03-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6c03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c03-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="d6c03-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="d6c03-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d6c03-107">Members</span></span>
|<span data-ttu-id="d6c03-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d6c03-108">Member</span></span>|<span data-ttu-id="d6c03-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d6c03-109">Value</span></span>|<span data-ttu-id="d6c03-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6c03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c03-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="d6c03-111">deviceDefault</span></span>|<span data-ttu-id="d6c03-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d6c03-112">0</span></span>|<span data-ttu-id="d6c03-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="d6c03-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d6c03-114">отключено</span><span class="sxs-lookup"><span data-stu-id="d6c03-114">disabled</span></span>|<span data-ttu-id="d6c03-115">1 </span><span class="sxs-lookup"><span data-stu-id="d6c03-115">1</span></span>|<span data-ttu-id="d6c03-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="d6c03-116">Disable packet queuing</span></span>|
|<span data-ttu-id="d6c03-117">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="d6c03-117">queueInbound</span></span>|<span data-ttu-id="d6c03-118">2 </span><span class="sxs-lookup"><span data-stu-id="d6c03-118">2</span></span>|<span data-ttu-id="d6c03-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="d6c03-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="d6c03-120">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="d6c03-120">queueOutbound</span></span>|<span data-ttu-id="d6c03-121">4</span><span class="sxs-lookup"><span data-stu-id="d6c03-121">3</span></span>|<span data-ttu-id="d6c03-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="d6c03-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="d6c03-123">куеуебос</span><span class="sxs-lookup"><span data-stu-id="d6c03-123">queueBoth</span></span>|<span data-ttu-id="d6c03-124">4 </span><span class="sxs-lookup"><span data-stu-id="d6c03-124">4</span></span>|<span data-ttu-id="d6c03-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="d6c03-125">Queue both inbound and outbound packets</span></span>|









