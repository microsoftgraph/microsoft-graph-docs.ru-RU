---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 110fffc41caa4efc6b7fbd9e1efe05f663cf8f85
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447726"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="eee0f-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="eee0f-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="eee0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eee0f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eee0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eee0f-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="eee0f-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="eee0f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="eee0f-107">Members</span></span>
|<span data-ttu-id="eee0f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="eee0f-108">Member</span></span>|<span data-ttu-id="eee0f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="eee0f-109">Value</span></span>|<span data-ttu-id="eee0f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eee0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee0f-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="eee0f-111">deviceDefault</span></span>|<span data-ttu-id="eee0f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="eee0f-112">0</span></span>|<span data-ttu-id="eee0f-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="eee0f-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="eee0f-114">отключено</span><span class="sxs-lookup"><span data-stu-id="eee0f-114">disabled</span></span>|<span data-ttu-id="eee0f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="eee0f-115">1</span></span>|<span data-ttu-id="eee0f-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="eee0f-116">Disable packet queuing</span></span>|
|<span data-ttu-id="eee0f-117">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="eee0f-117">queueInbound</span></span>|<span data-ttu-id="eee0f-118">2</span><span class="sxs-lookup"><span data-stu-id="eee0f-118">2</span></span>|<span data-ttu-id="eee0f-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="eee0f-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="eee0f-120">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="eee0f-120">queueOutbound</span></span>|<span data-ttu-id="eee0f-121">4</span><span class="sxs-lookup"><span data-stu-id="eee0f-121">3</span></span>|<span data-ttu-id="eee0f-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="eee0f-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="eee0f-123">куеуебос</span><span class="sxs-lookup"><span data-stu-id="eee0f-123">queueBoth</span></span>|<span data-ttu-id="eee0f-124">4 </span><span class="sxs-lookup"><span data-stu-id="eee0f-124">4</span></span>|<span data-ttu-id="eee0f-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="eee0f-125">Queue both inbound and outbound packets</span></span>|







