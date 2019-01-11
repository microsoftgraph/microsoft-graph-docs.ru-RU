---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1303287e521cf0b542047e8acaf122bc08a770a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823221"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="afb06-103">Тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="afb06-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="afb06-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afb06-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afb06-105">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="afb06-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="afb06-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="afb06-106">Members</span></span>
|<span data-ttu-id="afb06-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="afb06-107">Member</span></span>|<span data-ttu-id="afb06-108">Значение</span><span class="sxs-lookup"><span data-stu-id="afb06-108">Value</span></span>|<span data-ttu-id="afb06-109">Описание</span><span class="sxs-lookup"><span data-stu-id="afb06-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb06-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="afb06-110">deviceDefault</span></span>|<span data-ttu-id="afb06-111">0</span><span class="sxs-lookup"><span data-stu-id="afb06-111">0</span></span>|<span data-ttu-id="afb06-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="afb06-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="afb06-113">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="afb06-113">disabled</span></span>|<span data-ttu-id="afb06-114">1</span><span class="sxs-lookup"><span data-stu-id="afb06-114">1</span></span>|<span data-ttu-id="afb06-115">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="afb06-115">Disable packet queuing</span></span>|
|<span data-ttu-id="afb06-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="afb06-116">queueInbound</span></span>|<span data-ttu-id="afb06-117">2</span><span class="sxs-lookup"><span data-stu-id="afb06-117">2</span></span>|<span data-ttu-id="afb06-118">В очередь входящие зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="afb06-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="afb06-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="afb06-119">queueOutbound</span></span>|<span data-ttu-id="afb06-120">3</span><span class="sxs-lookup"><span data-stu-id="afb06-120">3</span></span>|<span data-ttu-id="afb06-121">Очередь расшифрован исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="afb06-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="afb06-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="afb06-122">queueBoth</span></span>|<span data-ttu-id="afb06-123">4</span><span class="sxs-lookup"><span data-stu-id="afb06-123">4</span></span>|<span data-ttu-id="afb06-124">Очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="afb06-124">Queue both inbound and outbound packets</span></span>|



