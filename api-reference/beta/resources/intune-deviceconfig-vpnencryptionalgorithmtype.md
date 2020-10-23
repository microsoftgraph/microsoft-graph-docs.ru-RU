---
title: тип перечисления Впненкриптионалгорисмтипе
description: Тип алгоритма шифрования для сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 420dff0b05cae2bb403b7f8746063fc3417c4a4f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728372"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="b4fcf-103">тип перечисления Впненкриптионалгорисмтипе</span><span class="sxs-lookup"><span data-stu-id="b4fcf-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="b4fcf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4fcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4fcf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4fcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4fcf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4fcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4fcf-107">Тип алгоритма шифрования для сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="b4fcf-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="b4fcf-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b4fcf-108">Members</span></span>
|<span data-ttu-id="b4fcf-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b4fcf-109">Member</span></span>|<span data-ttu-id="b4fcf-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b4fcf-110">Value</span></span>|<span data-ttu-id="b4fcf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4fcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4fcf-112">AES256</span><span class="sxs-lookup"><span data-stu-id="b4fcf-112">aes256</span></span>|<span data-ttu-id="b4fcf-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b4fcf-113">0</span></span>|<span data-ttu-id="b4fcf-114">AES — 256</span><span class="sxs-lookup"><span data-stu-id="b4fcf-114">AES-256</span></span>|
|<span data-ttu-id="b4fcf-115">3DES</span><span class="sxs-lookup"><span data-stu-id="b4fcf-115">des</span></span>|<span data-ttu-id="b4fcf-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b4fcf-116">1</span></span>|<span data-ttu-id="b4fcf-117">3DES</span><span class="sxs-lookup"><span data-stu-id="b4fcf-117">DES</span></span>|
|<span data-ttu-id="b4fcf-118">Тройн</span><span class="sxs-lookup"><span data-stu-id="b4fcf-118">tripleDes</span></span>|<span data-ttu-id="b4fcf-119">2</span><span class="sxs-lookup"><span data-stu-id="b4fcf-119">2</span></span>|<span data-ttu-id="b4fcf-120">СТАНДАРТ</span><span class="sxs-lookup"><span data-stu-id="b4fcf-120">3DES</span></span>|
|<span data-ttu-id="b4fcf-121">AES128</span><span class="sxs-lookup"><span data-stu-id="b4fcf-121">aes128</span></span>|<span data-ttu-id="b4fcf-122">4</span><span class="sxs-lookup"><span data-stu-id="b4fcf-122">3</span></span>|<span data-ttu-id="b4fcf-123">AES — 128</span><span class="sxs-lookup"><span data-stu-id="b4fcf-123">AES-128</span></span>|
|<span data-ttu-id="b4fcf-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="b4fcf-124">aes128Gcm</span></span>|<span data-ttu-id="b4fcf-125">4 </span><span class="sxs-lookup"><span data-stu-id="b4fcf-125">4</span></span>|<span data-ttu-id="b4fcf-126">AES-128-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="b4fcf-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="b4fcf-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="b4fcf-127">aes256Gcm</span></span>|<span data-ttu-id="b4fcf-128">5 </span><span class="sxs-lookup"><span data-stu-id="b4fcf-128">5</span></span>|<span data-ttu-id="b4fcf-129">AES-256-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="b4fcf-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="b4fcf-130">aes192</span><span class="sxs-lookup"><span data-stu-id="b4fcf-130">aes192</span></span>|<span data-ttu-id="b4fcf-131">6 </span><span class="sxs-lookup"><span data-stu-id="b4fcf-131">6</span></span>|<span data-ttu-id="b4fcf-132">AES — 192</span><span class="sxs-lookup"><span data-stu-id="b4fcf-132">AES-192</span></span>|
|<span data-ttu-id="b4fcf-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="b4fcf-133">aes192Gcm</span></span>|<span data-ttu-id="b4fcf-134">7 </span><span class="sxs-lookup"><span data-stu-id="b4fcf-134">7</span></span>|<span data-ttu-id="b4fcf-135">AES — 192 — GCM</span><span class="sxs-lookup"><span data-stu-id="b4fcf-135">AES-192-GCM</span></span>|





