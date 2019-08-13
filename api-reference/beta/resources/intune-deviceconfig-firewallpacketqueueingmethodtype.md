---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4222580a079fd37b381cdaf78e0b2985029ef34b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338142"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="4c30d-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="4c30d-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="4c30d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c30d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c30d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c30d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c30d-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="4c30d-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="4c30d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4c30d-107">Members</span></span>
|<span data-ttu-id="4c30d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4c30d-108">Member</span></span>|<span data-ttu-id="4c30d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4c30d-109">Value</span></span>|<span data-ttu-id="4c30d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c30d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c30d-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="4c30d-111">deviceDefault</span></span>|<span data-ttu-id="4c30d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4c30d-112">0</span></span>|<span data-ttu-id="4c30d-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="4c30d-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="4c30d-114">активирован</span><span class="sxs-lookup"><span data-stu-id="4c30d-114">disabled</span></span>|<span data-ttu-id="4c30d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4c30d-115">1</span></span>|<span data-ttu-id="4c30d-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="4c30d-116">Disable packet queuing</span></span>|
|<span data-ttu-id="4c30d-117">куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="4c30d-117">queueInbound</span></span>|<span data-ttu-id="4c30d-118">2</span><span class="sxs-lookup"><span data-stu-id="4c30d-118">2</span></span>|<span data-ttu-id="4c30d-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="4c30d-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="4c30d-120">куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="4c30d-120">queueOutbound</span></span>|<span data-ttu-id="4c30d-121">4</span><span class="sxs-lookup"><span data-stu-id="4c30d-121">3</span></span>|<span data-ttu-id="4c30d-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="4c30d-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="4c30d-123">куеуебос</span><span class="sxs-lookup"><span data-stu-id="4c30d-123">queueBoth</span></span>|<span data-ttu-id="4c30d-124">SP4</span><span class="sxs-lookup"><span data-stu-id="4c30d-124">4</span></span>|<span data-ttu-id="4c30d-125">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="4c30d-125">Queue both inbound and outbound packets</span></span>|



