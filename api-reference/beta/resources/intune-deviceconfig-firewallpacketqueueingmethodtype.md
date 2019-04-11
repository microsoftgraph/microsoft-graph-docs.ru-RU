---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2b83aa5d13ac170df1f9f99f8e430d10cdaba3e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803726"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="13566-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="13566-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="13566-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13566-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13566-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13566-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13566-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="13566-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="13566-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="13566-107">Members</span></span>
|<span data-ttu-id="13566-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="13566-108">Member</span></span>|<span data-ttu-id="13566-109">Значение</span><span class="sxs-lookup"><span data-stu-id="13566-109">Value</span></span>|<span data-ttu-id="13566-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13566-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13566-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="13566-111">deviceDefault</span></span>|<span data-ttu-id="13566-112">нуль</span><span class="sxs-lookup"><span data-stu-id="13566-112">0</span></span>|<span data-ttu-id="13566-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="13566-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="13566-114">активирован</span><span class="sxs-lookup"><span data-stu-id="13566-114">disabled</span></span>|<span data-ttu-id="13566-115">1,1</span><span class="sxs-lookup"><span data-stu-id="13566-115">1</span></span>|<span data-ttu-id="13566-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="13566-116">Disable packet queuing</span></span>|
|<span data-ttu-id="13566-117">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="13566-117">queueInbound</span></span>|<span data-ttu-id="13566-118">2</span><span class="sxs-lookup"><span data-stu-id="13566-118">2</span></span>|<span data-ttu-id="13566-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="13566-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="13566-120">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="13566-120">queueOutbound</span></span>|<span data-ttu-id="13566-121">4</span><span class="sxs-lookup"><span data-stu-id="13566-121">3</span></span>|<span data-ttu-id="13566-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="13566-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="13566-123">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="13566-123">queueBoth</span></span>|<span data-ttu-id="13566-124">SP4</span><span class="sxs-lookup"><span data-stu-id="13566-124">4</span></span>|<span data-ttu-id="13566-125">ПоСтановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="13566-125">Queue both inbound and outbound packets</span></span>|





