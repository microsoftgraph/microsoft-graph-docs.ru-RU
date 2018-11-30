---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
ms.openlocfilehash: f55b68780d3bec97fa48a32c7abd8e1cfb269755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079940"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="efb3a-103">Тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="efb3a-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="efb3a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="efb3a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efb3a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efb3a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="efb3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efb3a-107">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="efb3a-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="efb3a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="efb3a-108">Members</span></span>
|<span data-ttu-id="efb3a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="efb3a-109">Member</span></span>|<span data-ttu-id="efb3a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="efb3a-110">Value</span></span>|<span data-ttu-id="efb3a-111">Description</span><span class="sxs-lookup"><span data-stu-id="efb3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb3a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="efb3a-112">deviceDefault</span></span>|<span data-ttu-id="efb3a-113">0</span><span class="sxs-lookup"><span data-stu-id="efb3a-113">0</span></span>|<span data-ttu-id="efb3a-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="efb3a-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="efb3a-115">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="efb3a-115">disabled</span></span>|<span data-ttu-id="efb3a-116">1</span><span class="sxs-lookup"><span data-stu-id="efb3a-116">1</span></span>|<span data-ttu-id="efb3a-117">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="efb3a-117">Disable packet queuing</span></span>|
|<span data-ttu-id="efb3a-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="efb3a-118">queueInbound</span></span>|<span data-ttu-id="efb3a-119">2</span><span class="sxs-lookup"><span data-stu-id="efb3a-119">2</span></span>|<span data-ttu-id="efb3a-120">В очередь входящие зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="efb3a-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="efb3a-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="efb3a-121">queueOutbound</span></span>|<span data-ttu-id="efb3a-122">3</span><span class="sxs-lookup"><span data-stu-id="efb3a-122">3</span></span>|<span data-ttu-id="efb3a-123">Очередь расшифрован исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="efb3a-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="efb3a-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="efb3a-124">queueBoth</span></span>|<span data-ttu-id="efb3a-125">4</span><span class="sxs-lookup"><span data-stu-id="efb3a-125">4</span></span>|<span data-ttu-id="efb3a-126">Очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="efb3a-126">Queue both inbound and outbound packets</span></span>|





