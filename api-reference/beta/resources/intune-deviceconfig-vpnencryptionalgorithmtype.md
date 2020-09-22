---
title: тип перечисления Впненкриптионалгорисмтипе
description: Тип алгоритма шифрования для сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c8a07e6e1eb5190457b5c66630a9595264334cd1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049115"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="0444a-103">тип перечисления Впненкриптионалгорисмтипе</span><span class="sxs-lookup"><span data-stu-id="0444a-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="0444a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0444a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0444a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0444a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0444a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0444a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0444a-107">Тип алгоритма шифрования для сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="0444a-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="0444a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0444a-108">Members</span></span>
|<span data-ttu-id="0444a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0444a-109">Member</span></span>|<span data-ttu-id="0444a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0444a-110">Value</span></span>|<span data-ttu-id="0444a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0444a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0444a-112">AES256</span><span class="sxs-lookup"><span data-stu-id="0444a-112">aes256</span></span>|<span data-ttu-id="0444a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0444a-113">0</span></span>|<span data-ttu-id="0444a-114">AES — 256</span><span class="sxs-lookup"><span data-stu-id="0444a-114">AES-256</span></span>|
|<span data-ttu-id="0444a-115">3DES</span><span class="sxs-lookup"><span data-stu-id="0444a-115">des</span></span>|<span data-ttu-id="0444a-116">1 </span><span class="sxs-lookup"><span data-stu-id="0444a-116">1</span></span>|<span data-ttu-id="0444a-117">3DES</span><span class="sxs-lookup"><span data-stu-id="0444a-117">DES</span></span>|
|<span data-ttu-id="0444a-118">Тройн</span><span class="sxs-lookup"><span data-stu-id="0444a-118">tripleDes</span></span>|<span data-ttu-id="0444a-119">2 </span><span class="sxs-lookup"><span data-stu-id="0444a-119">2</span></span>|<span data-ttu-id="0444a-120">СТАНДАРТ</span><span class="sxs-lookup"><span data-stu-id="0444a-120">3DES</span></span>|
|<span data-ttu-id="0444a-121">AES128</span><span class="sxs-lookup"><span data-stu-id="0444a-121">aes128</span></span>|<span data-ttu-id="0444a-122">4</span><span class="sxs-lookup"><span data-stu-id="0444a-122">3</span></span>|<span data-ttu-id="0444a-123">AES — 128</span><span class="sxs-lookup"><span data-stu-id="0444a-123">AES-128</span></span>|
|<span data-ttu-id="0444a-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="0444a-124">aes128Gcm</span></span>|<span data-ttu-id="0444a-125">4 </span><span class="sxs-lookup"><span data-stu-id="0444a-125">4</span></span>|<span data-ttu-id="0444a-126">AES-128-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="0444a-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="0444a-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="0444a-127">aes256Gcm</span></span>|<span data-ttu-id="0444a-128">5 </span><span class="sxs-lookup"><span data-stu-id="0444a-128">5</span></span>|<span data-ttu-id="0444a-129">AES-256-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="0444a-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="0444a-130">aes192</span><span class="sxs-lookup"><span data-stu-id="0444a-130">aes192</span></span>|<span data-ttu-id="0444a-131">6 </span><span class="sxs-lookup"><span data-stu-id="0444a-131">6</span></span>|<span data-ttu-id="0444a-132">AES — 192</span><span class="sxs-lookup"><span data-stu-id="0444a-132">AES-192</span></span>|
|<span data-ttu-id="0444a-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="0444a-133">aes192Gcm</span></span>|<span data-ttu-id="0444a-134">7 </span><span class="sxs-lookup"><span data-stu-id="0444a-134">7</span></span>|<span data-ttu-id="0444a-135">AES — 192 — GCM</span><span class="sxs-lookup"><span data-stu-id="0444a-135">AES-192-GCM</span></span>|






