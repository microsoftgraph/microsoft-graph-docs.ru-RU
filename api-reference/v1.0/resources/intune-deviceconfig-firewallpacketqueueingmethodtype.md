---
title: брандмауэрPacketQueueingMethodType enum type
description: Возможные значения для брандмауэраPacketQueueingMethod
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a56e30f8b470271ea5fbb91765f7ea6814cbba14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758857"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="bb5e9-103">брандмауэрPacketQueueingMethodType enum type</span><span class="sxs-lookup"><span data-stu-id="bb5e9-103">firewallPacketQueueingMethodType enum type</span></span>

<span data-ttu-id="bb5e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb5e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb5e9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb5e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb5e9-106">Возможные значения для брандмауэраPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="bb5e9-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="bb5e9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bb5e9-107">Members</span></span>
|<span data-ttu-id="bb5e9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bb5e9-108">Member</span></span>|<span data-ttu-id="bb5e9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bb5e9-109">Value</span></span>|<span data-ttu-id="bb5e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb5e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb5e9-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="bb5e9-111">deviceDefault</span></span>|<span data-ttu-id="bb5e9-112">0</span><span class="sxs-lookup"><span data-stu-id="bb5e9-112">0</span></span>|<span data-ttu-id="bb5e9-113">Нет значения, настроенного Intune, не переопределять настроенное пользователем значение по умолчанию устройства</span><span class="sxs-lookup"><span data-stu-id="bb5e9-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="bb5e9-114">отключено</span><span class="sxs-lookup"><span data-stu-id="bb5e9-114">disabled</span></span>|<span data-ttu-id="bb5e9-115">1</span><span class="sxs-lookup"><span data-stu-id="bb5e9-115">1</span></span>|<span data-ttu-id="bb5e9-116">Отключение очередей пакетов</span><span class="sxs-lookup"><span data-stu-id="bb5e9-116">Disable packet queuing</span></span>|
|<span data-ttu-id="bb5e9-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="bb5e9-117">queueInbound</span></span>|<span data-ttu-id="bb5e9-118">2</span><span class="sxs-lookup"><span data-stu-id="bb5e9-118">2</span></span>|<span data-ttu-id="bb5e9-119">Входящие в очередь зашифрованные пакеты</span><span class="sxs-lookup"><span data-stu-id="bb5e9-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="bb5e9-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="bb5e9-120">queueOutbound</span></span>|<span data-ttu-id="bb5e9-121">3</span><span class="sxs-lookup"><span data-stu-id="bb5e9-121">3</span></span>|<span data-ttu-id="bb5e9-122">Расшифровка исходящие пакеты очереди для переададровки</span><span class="sxs-lookup"><span data-stu-id="bb5e9-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="bb5e9-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="bb5e9-123">queueBoth</span></span>|<span data-ttu-id="bb5e9-124">4 </span><span class="sxs-lookup"><span data-stu-id="bb5e9-124">4</span></span>|<span data-ttu-id="bb5e9-125">Очередь как входящие, так и исходящие пакеты</span><span class="sxs-lookup"><span data-stu-id="bb5e9-125">Queue both inbound and outbound packets</span></span>|




