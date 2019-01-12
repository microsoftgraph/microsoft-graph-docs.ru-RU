---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3700df6d2eaf0dd0d2dde8a3f4a90be2e3684951
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940101"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="1e595-103">Тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1e595-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="1e595-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e595-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e595-105">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1e595-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="1e595-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="1e595-106">Members</span></span>
|<span data-ttu-id="1e595-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="1e595-107">Member</span></span>|<span data-ttu-id="1e595-108">Значение</span><span class="sxs-lookup"><span data-stu-id="1e595-108">Value</span></span>|<span data-ttu-id="1e595-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e595-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e595-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1e595-110">deviceDefault</span></span>|<span data-ttu-id="1e595-111">0</span><span class="sxs-lookup"><span data-stu-id="1e595-111">0</span></span>|<span data-ttu-id="1e595-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="1e595-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1e595-113">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="1e595-113">disabled</span></span>|<span data-ttu-id="1e595-114">1</span><span class="sxs-lookup"><span data-stu-id="1e595-114">1</span></span>|<span data-ttu-id="1e595-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="1e595-115">Disable packet queuing</span></span>|
|<span data-ttu-id="1e595-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="1e595-116">queueInbound</span></span>|<span data-ttu-id="1e595-117">2</span><span class="sxs-lookup"><span data-stu-id="1e595-117">2</span></span>|<span data-ttu-id="1e595-118">В очередь входящие зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="1e595-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="1e595-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="1e595-119">queueOutbound</span></span>|<span data-ttu-id="1e595-120">3</span><span class="sxs-lookup"><span data-stu-id="1e595-120">3</span></span>|<span data-ttu-id="1e595-121">Очередь расшифрован исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="1e595-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="1e595-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="1e595-122">queueBoth</span></span>|<span data-ttu-id="1e595-123">4</span><span class="sxs-lookup"><span data-stu-id="1e595-123">4</span></span>|<span data-ttu-id="1e595-124">Очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="1e595-124">Queue both inbound and outbound packets</span></span>|



