---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d9b4591ceff59becfa6f9fb17d490c56d59c9703
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833014"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="df423-103">Тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="df423-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="df423-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="df423-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df423-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df423-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="df423-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df423-107">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="df423-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="df423-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="df423-108">Members</span></span>
|<span data-ttu-id="df423-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="df423-109">Member</span></span>|<span data-ttu-id="df423-110">Значение</span><span class="sxs-lookup"><span data-stu-id="df423-110">Value</span></span>|<span data-ttu-id="df423-111">Описание</span><span class="sxs-lookup"><span data-stu-id="df423-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df423-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="df423-112">deviceDefault</span></span>|<span data-ttu-id="df423-113">0</span><span class="sxs-lookup"><span data-stu-id="df423-113">0</span></span>|<span data-ttu-id="df423-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="df423-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="df423-115">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="df423-115">disabled</span></span>|<span data-ttu-id="df423-116">1</span><span class="sxs-lookup"><span data-stu-id="df423-116">1</span></span>|<span data-ttu-id="df423-117">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="df423-117">Disable packet queuing</span></span>|
|<span data-ttu-id="df423-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="df423-118">queueInbound</span></span>|<span data-ttu-id="df423-119">2</span><span class="sxs-lookup"><span data-stu-id="df423-119">2</span></span>|<span data-ttu-id="df423-120">В очередь входящие зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="df423-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="df423-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="df423-121">queueOutbound</span></span>|<span data-ttu-id="df423-122">3</span><span class="sxs-lookup"><span data-stu-id="df423-122">3</span></span>|<span data-ttu-id="df423-123">Очередь расшифрован исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="df423-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="df423-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="df423-124">queueBoth</span></span>|<span data-ttu-id="df423-125">4</span><span class="sxs-lookup"><span data-stu-id="df423-125">4</span></span>|<span data-ttu-id="df423-126">Очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="df423-126">Queue both inbound and outbound packets</span></span>|





