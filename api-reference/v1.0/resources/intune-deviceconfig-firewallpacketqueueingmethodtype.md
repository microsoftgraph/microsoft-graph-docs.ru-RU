---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c3ed6ebdb4386c8203964ad1072767ec580dce2a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359231"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="0945c-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="0945c-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="0945c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0945c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0945c-105">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="0945c-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="0945c-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="0945c-106">Members</span></span>
|<span data-ttu-id="0945c-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="0945c-107">Member</span></span>|<span data-ttu-id="0945c-108">Значение</span><span class="sxs-lookup"><span data-stu-id="0945c-108">Value</span></span>|<span data-ttu-id="0945c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0945c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0945c-110">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="0945c-110">deviceDefault</span></span>|<span data-ttu-id="0945c-111">нуль</span><span class="sxs-lookup"><span data-stu-id="0945c-111">0</span></span>|<span data-ttu-id="0945c-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="0945c-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="0945c-113">активирован</span><span class="sxs-lookup"><span data-stu-id="0945c-113">disabled</span></span>|<span data-ttu-id="0945c-114">1,1</span><span class="sxs-lookup"><span data-stu-id="0945c-114">1</span></span>|<span data-ttu-id="0945c-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="0945c-115">Disable packet queuing</span></span>|
|<span data-ttu-id="0945c-116">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="0945c-116">queueInbound</span></span>|<span data-ttu-id="0945c-117">2</span><span class="sxs-lookup"><span data-stu-id="0945c-117">2</span></span>|<span data-ttu-id="0945c-118">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="0945c-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="0945c-119">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="0945c-119">queueOutbound</span></span>|<span data-ttu-id="0945c-120">4</span><span class="sxs-lookup"><span data-stu-id="0945c-120">3</span></span>|<span data-ttu-id="0945c-121">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="0945c-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="0945c-122">куеуебос</span><span class="sxs-lookup"><span data-stu-id="0945c-122">queueBoth</span></span>|<span data-ttu-id="0945c-123">SP4</span><span class="sxs-lookup"><span data-stu-id="0945c-123">4</span></span>|<span data-ttu-id="0945c-124">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="0945c-124">Queue both inbound and outbound packets</span></span>|




