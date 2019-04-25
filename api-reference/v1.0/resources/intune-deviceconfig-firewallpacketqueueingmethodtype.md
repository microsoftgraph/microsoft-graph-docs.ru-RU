---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541310"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="d5f54-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d5f54-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="d5f54-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5f54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5f54-105">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="d5f54-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="d5f54-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d5f54-106">Members</span></span>
|<span data-ttu-id="d5f54-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d5f54-107">Member</span></span>|<span data-ttu-id="d5f54-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d5f54-108">Value</span></span>|<span data-ttu-id="d5f54-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d5f54-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5f54-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="d5f54-110">deviceDefault</span></span>|<span data-ttu-id="d5f54-111">нуль</span><span class="sxs-lookup"><span data-stu-id="d5f54-111">0</span></span>|<span data-ttu-id="d5f54-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="d5f54-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d5f54-113">активирован</span><span class="sxs-lookup"><span data-stu-id="d5f54-113">disabled</span></span>|<span data-ttu-id="d5f54-114">1 </span><span class="sxs-lookup"><span data-stu-id="d5f54-114">1</span></span>|<span data-ttu-id="d5f54-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="d5f54-115">Disable packet queuing</span></span>|
|<span data-ttu-id="d5f54-116">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="d5f54-116">queueInbound</span></span>|<span data-ttu-id="d5f54-117">2 </span><span class="sxs-lookup"><span data-stu-id="d5f54-117">2</span></span>|<span data-ttu-id="d5f54-118">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="d5f54-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="d5f54-119">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="d5f54-119">queueOutbound</span></span>|<span data-ttu-id="d5f54-120">3 </span><span class="sxs-lookup"><span data-stu-id="d5f54-120">3</span></span>|<span data-ttu-id="d5f54-121">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="d5f54-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="d5f54-122">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="d5f54-122">queueBoth</span></span>|<span data-ttu-id="d5f54-123">4 </span><span class="sxs-lookup"><span data-stu-id="d5f54-123">4</span></span>|<span data-ttu-id="d5f54-124">ПоСтановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="d5f54-124">Queue both inbound and outbound packets</span></span>|



