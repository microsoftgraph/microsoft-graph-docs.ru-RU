---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258928"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="b7c20-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="b7c20-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="b7c20-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7c20-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c20-105">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="b7c20-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="b7c20-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="b7c20-106">Members</span></span>
|<span data-ttu-id="b7c20-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="b7c20-107">Member</span></span>|<span data-ttu-id="b7c20-108">Значение</span><span class="sxs-lookup"><span data-stu-id="b7c20-108">Value</span></span>|<span data-ttu-id="b7c20-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c20-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c20-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="b7c20-110">deviceDefault</span></span>|<span data-ttu-id="b7c20-111">нуль</span><span class="sxs-lookup"><span data-stu-id="b7c20-111">0</span></span>|<span data-ttu-id="b7c20-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="b7c20-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b7c20-113">активирован</span><span class="sxs-lookup"><span data-stu-id="b7c20-113">disabled</span></span>|<span data-ttu-id="b7c20-114">1,1</span><span class="sxs-lookup"><span data-stu-id="b7c20-114">1</span></span>|<span data-ttu-id="b7c20-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="b7c20-115">Disable packet queuing</span></span>|
|<span data-ttu-id="b7c20-116">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="b7c20-116">queueInbound</span></span>|<span data-ttu-id="b7c20-117">2</span><span class="sxs-lookup"><span data-stu-id="b7c20-117">2</span></span>|<span data-ttu-id="b7c20-118">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="b7c20-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="b7c20-119">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="b7c20-119">queueOutbound</span></span>|<span data-ttu-id="b7c20-120">4</span><span class="sxs-lookup"><span data-stu-id="b7c20-120">3</span></span>|<span data-ttu-id="b7c20-121">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="b7c20-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="b7c20-122">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="b7c20-122">queueBoth</span></span>|<span data-ttu-id="b7c20-123">4</span><span class="sxs-lookup"><span data-stu-id="b7c20-123">4</span></span>|<span data-ttu-id="b7c20-124">ПоСтановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="b7c20-124">Queue both inbound and outbound packets</span></span>|



