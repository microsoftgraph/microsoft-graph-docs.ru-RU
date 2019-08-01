---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 49fdf3172879092a04c20d0d73724744a9ef0fb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031565"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="ab059-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="ab059-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="ab059-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab059-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab059-105">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="ab059-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="ab059-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ab059-106">Members</span></span>
|<span data-ttu-id="ab059-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ab059-107">Member</span></span>|<span data-ttu-id="ab059-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ab059-108">Value</span></span>|<span data-ttu-id="ab059-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ab059-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab059-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="ab059-110">deviceDefault</span></span>|<span data-ttu-id="ab059-111">нуль</span><span class="sxs-lookup"><span data-stu-id="ab059-111">0</span></span>|<span data-ttu-id="ab059-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="ab059-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ab059-113">активирован</span><span class="sxs-lookup"><span data-stu-id="ab059-113">disabled</span></span>|<span data-ttu-id="ab059-114">1,1</span><span class="sxs-lookup"><span data-stu-id="ab059-114">1</span></span>|<span data-ttu-id="ab059-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="ab059-115">Disable packet queuing</span></span>|
|<span data-ttu-id="ab059-116">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="ab059-116">queueInbound</span></span>|<span data-ttu-id="ab059-117">2</span><span class="sxs-lookup"><span data-stu-id="ab059-117">2</span></span>|<span data-ttu-id="ab059-118">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="ab059-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="ab059-119">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="ab059-119">queueOutbound</span></span>|<span data-ttu-id="ab059-120">4</span><span class="sxs-lookup"><span data-stu-id="ab059-120">3</span></span>|<span data-ttu-id="ab059-121">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="ab059-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="ab059-122">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="ab059-122">queueBoth</span></span>|<span data-ttu-id="ab059-123">SP4</span><span class="sxs-lookup"><span data-stu-id="ab059-123">4</span></span>|<span data-ttu-id="ab059-124">Постановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="ab059-124">Queue both inbound and outbound packets</span></span>|



