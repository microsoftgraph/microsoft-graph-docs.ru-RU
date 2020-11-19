---
title: тип перечисления Впненкриптионалгорисмтипе
description: Тип алгоритма шифрования для сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7813f66781f0443c570198248349c1bb08716fd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299662"
---
# <a name="vpnencryptionalgorithmtype-enum-type"></a><span data-ttu-id="0bf7f-103">тип перечисления Впненкриптионалгорисмтипе</span><span class="sxs-lookup"><span data-stu-id="0bf7f-103">vpnEncryptionAlgorithmType enum type</span></span>

<span data-ttu-id="0bf7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bf7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bf7f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bf7f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bf7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bf7f-107">Тип алгоритма шифрования для сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="0bf7f-107">The type of VPN security association encryption algorithm</span></span>

## <a name="members"></a><span data-ttu-id="0bf7f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0bf7f-108">Members</span></span>
|<span data-ttu-id="0bf7f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0bf7f-109">Member</span></span>|<span data-ttu-id="0bf7f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0bf7f-110">Value</span></span>|<span data-ttu-id="0bf7f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0bf7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bf7f-112">AES256</span><span class="sxs-lookup"><span data-stu-id="0bf7f-112">aes256</span></span>|<span data-ttu-id="0bf7f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0bf7f-113">0</span></span>|<span data-ttu-id="0bf7f-114">AES — 256</span><span class="sxs-lookup"><span data-stu-id="0bf7f-114">AES-256</span></span>|
|<span data-ttu-id="0bf7f-115">3DES</span><span class="sxs-lookup"><span data-stu-id="0bf7f-115">des</span></span>|<span data-ttu-id="0bf7f-116">1,1</span><span class="sxs-lookup"><span data-stu-id="0bf7f-116">1</span></span>|<span data-ttu-id="0bf7f-117">3DES</span><span class="sxs-lookup"><span data-stu-id="0bf7f-117">DES</span></span>|
|<span data-ttu-id="0bf7f-118">Тройн</span><span class="sxs-lookup"><span data-stu-id="0bf7f-118">tripleDes</span></span>|<span data-ttu-id="0bf7f-119">2</span><span class="sxs-lookup"><span data-stu-id="0bf7f-119">2</span></span>|<span data-ttu-id="0bf7f-120">СТАНДАРТ</span><span class="sxs-lookup"><span data-stu-id="0bf7f-120">3DES</span></span>|
|<span data-ttu-id="0bf7f-121">AES128</span><span class="sxs-lookup"><span data-stu-id="0bf7f-121">aes128</span></span>|<span data-ttu-id="0bf7f-122">4</span><span class="sxs-lookup"><span data-stu-id="0bf7f-122">3</span></span>|<span data-ttu-id="0bf7f-123">AES — 128</span><span class="sxs-lookup"><span data-stu-id="0bf7f-123">AES-128</span></span>|
|<span data-ttu-id="0bf7f-124">aes128Gcm</span><span class="sxs-lookup"><span data-stu-id="0bf7f-124">aes128Gcm</span></span>|<span data-ttu-id="0bf7f-125">4 </span><span class="sxs-lookup"><span data-stu-id="0bf7f-125">4</span></span>|<span data-ttu-id="0bf7f-126">AES-128-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="0bf7f-126">AES-128-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="0bf7f-127">aes256Gcm</span><span class="sxs-lookup"><span data-stu-id="0bf7f-127">aes256Gcm</span></span>|<span data-ttu-id="0bf7f-128">5 </span><span class="sxs-lookup"><span data-stu-id="0bf7f-128">5</span></span>|<span data-ttu-id="0bf7f-129">AES-256-GCM (16-октет ИКВ)</span><span class="sxs-lookup"><span data-stu-id="0bf7f-129">AES-256-GCM (16-octet ICV)</span></span>|
|<span data-ttu-id="0bf7f-130">aes192</span><span class="sxs-lookup"><span data-stu-id="0bf7f-130">aes192</span></span>|<span data-ttu-id="0bf7f-131">6 </span><span class="sxs-lookup"><span data-stu-id="0bf7f-131">6</span></span>|<span data-ttu-id="0bf7f-132">AES — 192</span><span class="sxs-lookup"><span data-stu-id="0bf7f-132">AES-192</span></span>|
|<span data-ttu-id="0bf7f-133">aes192Gcm</span><span class="sxs-lookup"><span data-stu-id="0bf7f-133">aes192Gcm</span></span>|<span data-ttu-id="0bf7f-134">7 </span><span class="sxs-lookup"><span data-stu-id="0bf7f-134">7</span></span>|<span data-ttu-id="0bf7f-135">AES — 192 — GCM</span><span class="sxs-lookup"><span data-stu-id="0bf7f-135">AES-192-GCM</span></span>|




