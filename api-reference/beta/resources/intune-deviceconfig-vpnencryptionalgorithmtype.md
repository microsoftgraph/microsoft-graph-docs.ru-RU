---
title: тип перечисления Впненкриптионалгорисмтипе
description: Тип алгоритма шифрования для сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b8a14effae7c95605529c0d0b12eb45f51708c43
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788161"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="edb35-103">тип перечисления Впненкриптионалгорисмтипе</span><span class="sxs-lookup"><span data-stu-id="edb35-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="edb35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edb35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edb35-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edb35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edb35-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edb35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edb35-107">Тип алгоритма шифрования для сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="edb35-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="edb35-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="edb35-108">Members</span></span>
|<span data-ttu-id="edb35-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="edb35-109">Member</span></span>|<span data-ttu-id="edb35-110">Значение</span><span class="sxs-lookup"><span data-stu-id="edb35-110">Value</span></span>|<span data-ttu-id="edb35-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edb35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edb35-112">AES256</span><span class="sxs-lookup"><span data-stu-id="edb35-112">aes256</span></span>|<span data-ttu-id="edb35-113">нуль</span><span class="sxs-lookup"><span data-stu-id="edb35-113">0</span></span>|<span data-ttu-id="edb35-114">AES — 256</span><span class="sxs-lookup"><span data-stu-id="edb35-114">AES-256</span></span>|
|<span data-ttu-id="edb35-115">3DES</span><span class="sxs-lookup"><span data-stu-id="edb35-115">des</span></span>|<span data-ttu-id="edb35-116">1 </span><span class="sxs-lookup"><span data-stu-id="edb35-116">1</span></span>|<span data-ttu-id="edb35-117">3DES</span><span class="sxs-lookup"><span data-stu-id="edb35-117">DES</span></span>|
|<span data-ttu-id="edb35-118">Тройн</span><span class="sxs-lookup"><span data-stu-id="edb35-118">tripleDes</span></span>|<span data-ttu-id="edb35-119">2</span><span class="sxs-lookup"><span data-stu-id="edb35-119">2</span></span>|<span data-ttu-id="edb35-120">СТАНДАРТ</span><span class="sxs-lookup"><span data-stu-id="edb35-120">3DES</span></span>|
|<span data-ttu-id="edb35-121">AES128</span><span class="sxs-lookup"><span data-stu-id="edb35-121">aes128</span></span>|<span data-ttu-id="edb35-122">4</span><span class="sxs-lookup"><span data-stu-id="edb35-122">3</span></span>|<span data-ttu-id="edb35-123">AES — 128</span><span class="sxs-lookup"><span data-stu-id="edb35-123">AES-128</span></span>|
|<span data-ttu-id="edb35-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="edb35-124">aes128Gcm</span></span>|<span data-ttu-id="edb35-125">4 </span><span class="sxs-lookup"><span data-stu-id="edb35-125">4</span></span>|<span data-ttu-id="edb35-126">AES-128-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="edb35-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="edb35-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="edb35-127">aes256Gcm</span></span>|<span data-ttu-id="edb35-128">5 </span><span class="sxs-lookup"><span data-stu-id="edb35-128">5</span></span>|<span data-ttu-id="edb35-129">AES-256-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="edb35-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="edb35-130">aes192</span><span class="sxs-lookup"><span data-stu-id="edb35-130">aes192</span></span>|<span data-ttu-id="edb35-131">6 </span><span class="sxs-lookup"><span data-stu-id="edb35-131">6</span></span>|<span data-ttu-id="edb35-132">AES — 192</span><span class="sxs-lookup"><span data-stu-id="edb35-132">AES-192</span></span>|
|<span data-ttu-id="edb35-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="edb35-133">aes192Gcm</span></span>|<span data-ttu-id="edb35-134">7 </span><span class="sxs-lookup"><span data-stu-id="edb35-134">7</span></span>|<span data-ttu-id="edb35-135">AES — 192 — GCM</span><span class="sxs-lookup"><span data-stu-id="edb35-135">AES-192-GCM</span></span>|



