---
title: тип перечисления Девицеманажементексчанжеакцессстатереасон
description: Причина состояния доступа к Exchange для устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bf3b6d3200ab461877b90dda2226437c863b4d0c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453992"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="a2a60-103">тип перечисления Девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="a2a60-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="a2a60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2a60-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2a60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2a60-106">Причина состояния доступа к Exchange для устройства.</span><span class="sxs-lookup"><span data-stu-id="a2a60-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="a2a60-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a2a60-107">Members</span></span>
|<span data-ttu-id="a2a60-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a2a60-108">Member</span></span>|<span data-ttu-id="a2a60-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a2a60-109">Value</span></span>|<span data-ttu-id="a2a60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2a60-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2a60-111">нет</span><span class="sxs-lookup"><span data-stu-id="a2a60-111">none</span></span>|<span data-ttu-id="a2a60-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a2a60-112">0</span></span>|<span data-ttu-id="a2a60-113">Не обнаружена Причина состояния доступа в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="a2a60-114">unknown</span><span class="sxs-lookup"><span data-stu-id="a2a60-114">unknown</span></span>|<span data-ttu-id="a2a60-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a2a60-115">1</span></span>|<span data-ttu-id="a2a60-116">Причина неизвестного состояния доступа</span><span class="sxs-lookup"><span data-stu-id="a2a60-116">Unknown access state reason</span></span>|
|<span data-ttu-id="a2a60-117">ексчанжеглобалруле</span><span class="sxs-lookup"><span data-stu-id="a2a60-117">exchangeGlobalRule</span></span>|<span data-ttu-id="a2a60-118">2</span><span class="sxs-lookup"><span data-stu-id="a2a60-118">2</span></span>|<span data-ttu-id="a2a60-119">Состояние доступа определяется глобальным правилом Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="a2a60-120">ексчанжеиндивидуалруле</span><span class="sxs-lookup"><span data-stu-id="a2a60-120">exchangeIndividualRule</span></span>|<span data-ttu-id="a2a60-121">4</span><span class="sxs-lookup"><span data-stu-id="a2a60-121">3</span></span>|<span data-ttu-id="a2a60-122">Состояние доступа определяется индивидуальной правилом Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="a2a60-123">ексчанжедевицеруле</span><span class="sxs-lookup"><span data-stu-id="a2a60-123">exchangeDeviceRule</span></span>|<span data-ttu-id="a2a60-124">4 </span><span class="sxs-lookup"><span data-stu-id="a2a60-124">4</span></span>|<span data-ttu-id="a2a60-125">Состояние доступа определяется правилом устройства Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="a2a60-126">ексчанжеупграде</span><span class="sxs-lookup"><span data-stu-id="a2a60-126">exchangeUpgrade</span></span>|<span data-ttu-id="a2a60-127">5 </span><span class="sxs-lookup"><span data-stu-id="a2a60-127">5</span></span>|<span data-ttu-id="a2a60-128">Состояние доступа из-за обновления Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="a2a60-129">ексчанжемаилбоксполици</span><span class="sxs-lookup"><span data-stu-id="a2a60-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="a2a60-130">6 </span><span class="sxs-lookup"><span data-stu-id="a2a60-130">6</span></span>|<span data-ttu-id="a2a60-131">Состояние доступа определяется политикой почтовых ящиков Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="a2a60-132">остальные</span><span class="sxs-lookup"><span data-stu-id="a2a60-132">other</span></span>|<span data-ttu-id="a2a60-133">7 </span><span class="sxs-lookup"><span data-stu-id="a2a60-133">7</span></span>|<span data-ttu-id="a2a60-134">Состояние доступа определяется Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a60-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="a2a60-135">совместимо</span><span class="sxs-lookup"><span data-stu-id="a2a60-135">compliant</span></span>|<span data-ttu-id="a2a60-136">8 </span><span class="sxs-lookup"><span data-stu-id="a2a60-136">8</span></span>|<span data-ttu-id="a2a60-137">Состояние доступа, предоставленное запросом на соответствие</span><span class="sxs-lookup"><span data-stu-id="a2a60-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="a2a60-138">ноткомплиант</span><span class="sxs-lookup"><span data-stu-id="a2a60-138">notCompliant</span></span>|<span data-ttu-id="a2a60-139">9 </span><span class="sxs-lookup"><span data-stu-id="a2a60-139">9</span></span>|<span data-ttu-id="a2a60-140">Состояние доступа отозвано с помощью запроса на соответствие</span><span class="sxs-lookup"><span data-stu-id="a2a60-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="a2a60-141">нотенроллед</span><span class="sxs-lookup"><span data-stu-id="a2a60-141">notEnrolled</span></span>|<span data-ttu-id="a2a60-142">10 </span><span class="sxs-lookup"><span data-stu-id="a2a60-142">10</span></span>|<span data-ttu-id="a2a60-143">Состояние доступа, аннулированное запросом управления</span><span class="sxs-lookup"><span data-stu-id="a2a60-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="a2a60-144">ункновнлокатион</span><span class="sxs-lookup"><span data-stu-id="a2a60-144">unknownLocation</span></span>|<span data-ttu-id="a2a60-145">12</span><span class="sxs-lookup"><span data-stu-id="a2a60-145">12</span></span>|<span data-ttu-id="a2a60-146">Состояние доступа в связи с неизвестным расположением</span><span class="sxs-lookup"><span data-stu-id="a2a60-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="a2a60-147">мфарекуиред</span><span class="sxs-lookup"><span data-stu-id="a2a60-147">mfaRequired</span></span>|<span data-ttu-id="a2a60-148">13 </span><span class="sxs-lookup"><span data-stu-id="a2a60-148">13</span></span>|<span data-ttu-id="a2a60-149">Состояние доступа из-за вызова MFA</span><span class="sxs-lookup"><span data-stu-id="a2a60-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="a2a60-150">азуреадблоккдуетоакцессполици</span><span class="sxs-lookup"><span data-stu-id="a2a60-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="a2a60-151">14 </span><span class="sxs-lookup"><span data-stu-id="a2a60-151">14</span></span>|<span data-ttu-id="a2a60-152">Состояние доступа, отозванное политикой доступа AAD</span><span class="sxs-lookup"><span data-stu-id="a2a60-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="a2a60-153">компромиседпассворд</span><span class="sxs-lookup"><span data-stu-id="a2a60-153">compromisedPassword</span></span>|<span data-ttu-id="a2a60-154">15 </span><span class="sxs-lookup"><span data-stu-id="a2a60-154">15</span></span>|<span data-ttu-id="a2a60-155">Состояние доступа отозвано с помощью скомпрометированного пароля</span><span class="sxs-lookup"><span data-stu-id="a2a60-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="a2a60-156">девиценоткновнвисманажедапп</span><span class="sxs-lookup"><span data-stu-id="a2a60-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="a2a60-157">16 </span><span class="sxs-lookup"><span data-stu-id="a2a60-157">16</span></span>|<span data-ttu-id="a2a60-158">Состояние доступа, отозванное с помощью вызова управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="a2a60-158">Access state revoked by managed application challenge</span></span>|







