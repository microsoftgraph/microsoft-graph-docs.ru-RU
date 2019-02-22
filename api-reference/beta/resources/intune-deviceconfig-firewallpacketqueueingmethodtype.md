---
title: тип перечисления Фиреваллпаккеткуеуеингмесодтипе
description: Возможные значения для Фиреваллпаккеткуеуеингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1b8543df5fa2a50cfdfa56c7cb2d96199ba44e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172207"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="8746b-103">тип перечисления Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="8746b-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="8746b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8746b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8746b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8746b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8746b-106">Возможные значения для Фиреваллпаккеткуеуеингмесод</span><span class="sxs-lookup"><span data-stu-id="8746b-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="8746b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8746b-107">Members</span></span>
|<span data-ttu-id="8746b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8746b-108">Member</span></span>|<span data-ttu-id="8746b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8746b-109">Value</span></span>|<span data-ttu-id="8746b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8746b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8746b-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="8746b-111">deviceDefault</span></span>|<span data-ttu-id="8746b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8746b-112">0</span></span>|<span data-ttu-id="8746b-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="8746b-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="8746b-114">активирован</span><span class="sxs-lookup"><span data-stu-id="8746b-114">disabled</span></span>|<span data-ttu-id="8746b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8746b-115">1</span></span>|<span data-ttu-id="8746b-116">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="8746b-116">Disable packet queuing</span></span>|
|<span data-ttu-id="8746b-117">Куеуеинбаунд</span><span class="sxs-lookup"><span data-stu-id="8746b-117">queueInbound</span></span>|<span data-ttu-id="8746b-118">2</span><span class="sxs-lookup"><span data-stu-id="8746b-118">2</span></span>|<span data-ttu-id="8746b-119">Очередь входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="8746b-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="8746b-120">Куеуеаутбаунд</span><span class="sxs-lookup"><span data-stu-id="8746b-120">queueOutbound</span></span>|<span data-ttu-id="8746b-121">4</span><span class="sxs-lookup"><span data-stu-id="8746b-121">3</span></span>|<span data-ttu-id="8746b-122">Очередь расшифрованных исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="8746b-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="8746b-123">Куеуебос</span><span class="sxs-lookup"><span data-stu-id="8746b-123">queueBoth</span></span>|<span data-ttu-id="8746b-124">4</span><span class="sxs-lookup"><span data-stu-id="8746b-124">4</span></span>|<span data-ttu-id="8746b-125">ПоСтановка в очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="8746b-125">Queue both inbound and outbound packets</span></span>|




