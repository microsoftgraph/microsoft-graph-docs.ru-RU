---
title: тип перечисления Девицеманажементексчанжеакцессстатереасон
description: Причина состояния доступа к Exchange для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 37ce7d40ef2f8ea6cc729b25bcfc9b66480fdf6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091175"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="ce19a-103">тип перечисления Девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="ce19a-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="ce19a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce19a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce19a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce19a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce19a-106">Причина состояния доступа к Exchange для устройства.</span><span class="sxs-lookup"><span data-stu-id="ce19a-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="ce19a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ce19a-107">Members</span></span>
|<span data-ttu-id="ce19a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ce19a-108">Member</span></span>|<span data-ttu-id="ce19a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ce19a-109">Value</span></span>|<span data-ttu-id="ce19a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ce19a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce19a-111">Нет</span><span class="sxs-lookup"><span data-stu-id="ce19a-111">none</span></span>|<span data-ttu-id="ce19a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ce19a-112">0</span></span>|<span data-ttu-id="ce19a-113">Не обнаружена Причина состояния доступа в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="ce19a-114">unknown</span><span class="sxs-lookup"><span data-stu-id="ce19a-114">unknown</span></span>|<span data-ttu-id="ce19a-115">1 </span><span class="sxs-lookup"><span data-stu-id="ce19a-115">1</span></span>|<span data-ttu-id="ce19a-116">Причина неизвестного состояния доступа</span><span class="sxs-lookup"><span data-stu-id="ce19a-116">Unknown access state reason</span></span>|
|<span data-ttu-id="ce19a-117">ексчанжеглобалруле</span><span class="sxs-lookup"><span data-stu-id="ce19a-117">exchangeGlobalRule</span></span>|<span data-ttu-id="ce19a-118">2 </span><span class="sxs-lookup"><span data-stu-id="ce19a-118">2</span></span>|<span data-ttu-id="ce19a-119">Состояние доступа определяется глобальным правилом Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="ce19a-120">ексчанжеиндивидуалруле</span><span class="sxs-lookup"><span data-stu-id="ce19a-120">exchangeIndividualRule</span></span>|<span data-ttu-id="ce19a-121">4</span><span class="sxs-lookup"><span data-stu-id="ce19a-121">3</span></span>|<span data-ttu-id="ce19a-122">Состояние доступа определяется индивидуальной правилом Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="ce19a-123">ексчанжедевицеруле</span><span class="sxs-lookup"><span data-stu-id="ce19a-123">exchangeDeviceRule</span></span>|<span data-ttu-id="ce19a-124">4 </span><span class="sxs-lookup"><span data-stu-id="ce19a-124">4</span></span>|<span data-ttu-id="ce19a-125">Состояние доступа определяется правилом устройства Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="ce19a-126">ексчанжеупграде</span><span class="sxs-lookup"><span data-stu-id="ce19a-126">exchangeUpgrade</span></span>|<span data-ttu-id="ce19a-127">5 </span><span class="sxs-lookup"><span data-stu-id="ce19a-127">5</span></span>|<span data-ttu-id="ce19a-128">Состояние доступа из-за обновления Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="ce19a-129">ексчанжемаилбоксполици</span><span class="sxs-lookup"><span data-stu-id="ce19a-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="ce19a-130">6 </span><span class="sxs-lookup"><span data-stu-id="ce19a-130">6</span></span>|<span data-ttu-id="ce19a-131">Состояние доступа определяется политикой почтовых ящиков Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="ce19a-132">остальные</span><span class="sxs-lookup"><span data-stu-id="ce19a-132">other</span></span>|<span data-ttu-id="ce19a-133">7 </span><span class="sxs-lookup"><span data-stu-id="ce19a-133">7</span></span>|<span data-ttu-id="ce19a-134">Состояние доступа определяется Exchange</span><span class="sxs-lookup"><span data-stu-id="ce19a-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="ce19a-135">совместимо</span><span class="sxs-lookup"><span data-stu-id="ce19a-135">compliant</span></span>|<span data-ttu-id="ce19a-136">8 </span><span class="sxs-lookup"><span data-stu-id="ce19a-136">8</span></span>|<span data-ttu-id="ce19a-137">Состояние доступа, предоставленное запросом на соответствие</span><span class="sxs-lookup"><span data-stu-id="ce19a-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="ce19a-138">ноткомплиант</span><span class="sxs-lookup"><span data-stu-id="ce19a-138">notCompliant</span></span>|<span data-ttu-id="ce19a-139">9 </span><span class="sxs-lookup"><span data-stu-id="ce19a-139">9</span></span>|<span data-ttu-id="ce19a-140">Состояние доступа отозвано с помощью запроса на соответствие</span><span class="sxs-lookup"><span data-stu-id="ce19a-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="ce19a-141">нотенроллед</span><span class="sxs-lookup"><span data-stu-id="ce19a-141">notEnrolled</span></span>|<span data-ttu-id="ce19a-142">10 </span><span class="sxs-lookup"><span data-stu-id="ce19a-142">10</span></span>|<span data-ttu-id="ce19a-143">Состояние доступа, аннулированное запросом управления</span><span class="sxs-lookup"><span data-stu-id="ce19a-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="ce19a-144">ункновнлокатион</span><span class="sxs-lookup"><span data-stu-id="ce19a-144">unknownLocation</span></span>|<span data-ttu-id="ce19a-145">12 </span><span class="sxs-lookup"><span data-stu-id="ce19a-145">12</span></span>|<span data-ttu-id="ce19a-146">Состояние доступа в связи с неизвестным расположением</span><span class="sxs-lookup"><span data-stu-id="ce19a-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="ce19a-147">мфарекуиред</span><span class="sxs-lookup"><span data-stu-id="ce19a-147">mfaRequired</span></span>|<span data-ttu-id="ce19a-148">13 </span><span class="sxs-lookup"><span data-stu-id="ce19a-148">13</span></span>|<span data-ttu-id="ce19a-149">Состояние доступа из-за вызова MFA</span><span class="sxs-lookup"><span data-stu-id="ce19a-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="ce19a-150">азуреадблоккдуетоакцессполици</span><span class="sxs-lookup"><span data-stu-id="ce19a-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="ce19a-151">14 </span><span class="sxs-lookup"><span data-stu-id="ce19a-151">14</span></span>|<span data-ttu-id="ce19a-152">Состояние доступа, отозванное политикой доступа AAD</span><span class="sxs-lookup"><span data-stu-id="ce19a-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="ce19a-153">компромиседпассворд</span><span class="sxs-lookup"><span data-stu-id="ce19a-153">compromisedPassword</span></span>|<span data-ttu-id="ce19a-154">15 </span><span class="sxs-lookup"><span data-stu-id="ce19a-154">15</span></span>|<span data-ttu-id="ce19a-155">Состояние доступа отозвано с помощью скомпрометированного пароля</span><span class="sxs-lookup"><span data-stu-id="ce19a-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="ce19a-156">девиценоткновнвисманажедапп</span><span class="sxs-lookup"><span data-stu-id="ce19a-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="ce19a-157">16 </span><span class="sxs-lookup"><span data-stu-id="ce19a-157">16</span></span>|<span data-ttu-id="ce19a-158">Состояние доступа, отозванное с помощью вызова управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="ce19a-158">Access state revoked by managed application challenge</span></span>|









