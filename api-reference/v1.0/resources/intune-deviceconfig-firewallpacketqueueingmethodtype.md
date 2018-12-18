---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
author: tfitzmac
ms.openlocfilehash: 9f3d63b7e58b6f9c5ba369c3ceb12d06704c4725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304559"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="fd0e7-103">Тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="fd0e7-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="fd0e7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd0e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd0e7-105">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="fd0e7-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="fd0e7-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="fd0e7-106">Members</span></span>
|<span data-ttu-id="fd0e7-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="fd0e7-107">Member</span></span>|<span data-ttu-id="fd0e7-108">Значение</span><span class="sxs-lookup"><span data-stu-id="fd0e7-108">Value</span></span>|<span data-ttu-id="fd0e7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd0e7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd0e7-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fd0e7-110">deviceDefault</span></span>|<span data-ttu-id="fd0e7-111">0</span><span class="sxs-lookup"><span data-stu-id="fd0e7-111">0</span></span>|<span data-ttu-id="fd0e7-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="fd0e7-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="fd0e7-113">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="fd0e7-113">disabled</span></span>|<span data-ttu-id="fd0e7-114">1</span><span class="sxs-lookup"><span data-stu-id="fd0e7-114">1</span></span>|<span data-ttu-id="fd0e7-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="fd0e7-115">Disable packet queuing</span></span>|
|<span data-ttu-id="fd0e7-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="fd0e7-116">queueInbound</span></span>|<span data-ttu-id="fd0e7-117">2</span><span class="sxs-lookup"><span data-stu-id="fd0e7-117">2</span></span>|<span data-ttu-id="fd0e7-118">В очередь входящие зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="fd0e7-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="fd0e7-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="fd0e7-119">queueOutbound</span></span>|<span data-ttu-id="fd0e7-120">3</span><span class="sxs-lookup"><span data-stu-id="fd0e7-120">3</span></span>|<span data-ttu-id="fd0e7-121">Очередь расшифрован исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="fd0e7-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="fd0e7-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="fd0e7-122">queueBoth</span></span>|<span data-ttu-id="fd0e7-123">4</span><span class="sxs-lookup"><span data-stu-id="fd0e7-123">4</span></span>|<span data-ttu-id="fd0e7-124">Очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="fd0e7-124">Queue both inbound and outbound packets</span></span>|



