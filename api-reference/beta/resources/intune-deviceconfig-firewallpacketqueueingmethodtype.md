---
title: Тип перечисления firewallPacketQueueingMethodType
description: Возможные значения для firewallPacketQueueingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc40b93eebc17b1d1abcd9c317da1ffa538512a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425759"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="bd26a-103">Тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="bd26a-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="bd26a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd26a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd26a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd26a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd26a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd26a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd26a-107">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="bd26a-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="bd26a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bd26a-108">Members</span></span>
|<span data-ttu-id="bd26a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bd26a-109">Member</span></span>|<span data-ttu-id="bd26a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bd26a-110">Value</span></span>|<span data-ttu-id="bd26a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd26a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd26a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="bd26a-112">deviceDefault</span></span>|<span data-ttu-id="bd26a-113">0</span><span class="sxs-lookup"><span data-stu-id="bd26a-113">0</span></span>|<span data-ttu-id="bd26a-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="bd26a-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="bd26a-115">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="bd26a-115">disabled</span></span>|<span data-ttu-id="bd26a-116">1</span><span class="sxs-lookup"><span data-stu-id="bd26a-116">1</span></span>|<span data-ttu-id="bd26a-117">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="bd26a-117">Disable packet queuing</span></span>|
|<span data-ttu-id="bd26a-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="bd26a-118">queueInbound</span></span>|<span data-ttu-id="bd26a-119">2</span><span class="sxs-lookup"><span data-stu-id="bd26a-119">2</span></span>|<span data-ttu-id="bd26a-120">В очередь входящие зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="bd26a-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="bd26a-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="bd26a-121">queueOutbound</span></span>|<span data-ttu-id="bd26a-122">3</span><span class="sxs-lookup"><span data-stu-id="bd26a-122">3</span></span>|<span data-ttu-id="bd26a-123">Очередь расшифрован исходящих пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="bd26a-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="bd26a-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="bd26a-124">queueBoth</span></span>|<span data-ttu-id="bd26a-125">4</span><span class="sxs-lookup"><span data-stu-id="bd26a-125">4</span></span>|<span data-ttu-id="bd26a-126">Очередь входящих и исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="bd26a-126">Queue both inbound and outbound packets</span></span>|




