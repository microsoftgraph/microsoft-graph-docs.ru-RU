---
title: тип перечисления Девицеманажементексчанжеакцессстатереасон
description: Причина состояния доступа к Exchange для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0b2e45192ee953ca38e3738c87ee3c0714d0dfdd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060155"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="c495f-103">тип перечисления Девицеманажементексчанжеакцессстатереасон</span><span class="sxs-lookup"><span data-stu-id="c495f-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="c495f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c495f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c495f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c495f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c495f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c495f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c495f-107">Причина состояния доступа к Exchange для устройства.</span><span class="sxs-lookup"><span data-stu-id="c495f-107">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="c495f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c495f-108">Members</span></span>
|<span data-ttu-id="c495f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c495f-109">Member</span></span>|<span data-ttu-id="c495f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c495f-110">Value</span></span>|<span data-ttu-id="c495f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c495f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c495f-112">Нет</span><span class="sxs-lookup"><span data-stu-id="c495f-112">none</span></span>|<span data-ttu-id="c495f-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c495f-113">0</span></span>|<span data-ttu-id="c495f-114">Не обнаружена Причина состояния доступа в Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-114">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="c495f-115">unknown</span><span class="sxs-lookup"><span data-stu-id="c495f-115">unknown</span></span>|<span data-ttu-id="c495f-116">1 </span><span class="sxs-lookup"><span data-stu-id="c495f-116">1</span></span>|<span data-ttu-id="c495f-117">Причина неизвестного состояния доступа</span><span class="sxs-lookup"><span data-stu-id="c495f-117">Unknown access state reason</span></span>|
|<span data-ttu-id="c495f-118">ексчанжеглобалруле</span><span class="sxs-lookup"><span data-stu-id="c495f-118">exchangeGlobalRule</span></span>|<span data-ttu-id="c495f-119">2 </span><span class="sxs-lookup"><span data-stu-id="c495f-119">2</span></span>|<span data-ttu-id="c495f-120">Состояние доступа определяется глобальным правилом Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-120">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="c495f-121">ексчанжеиндивидуалруле</span><span class="sxs-lookup"><span data-stu-id="c495f-121">exchangeIndividualRule</span></span>|<span data-ttu-id="c495f-122">4</span><span class="sxs-lookup"><span data-stu-id="c495f-122">3</span></span>|<span data-ttu-id="c495f-123">Состояние доступа определяется индивидуальной правилом Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-123">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="c495f-124">ексчанжедевицеруле</span><span class="sxs-lookup"><span data-stu-id="c495f-124">exchangeDeviceRule</span></span>|<span data-ttu-id="c495f-125">4 </span><span class="sxs-lookup"><span data-stu-id="c495f-125">4</span></span>|<span data-ttu-id="c495f-126">Состояние доступа определяется правилом устройства Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-126">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="c495f-127">ексчанжеупграде</span><span class="sxs-lookup"><span data-stu-id="c495f-127">exchangeUpgrade</span></span>|<span data-ttu-id="c495f-128">5 </span><span class="sxs-lookup"><span data-stu-id="c495f-128">5</span></span>|<span data-ttu-id="c495f-129">Состояние доступа из-за обновления Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-129">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="c495f-130">ексчанжемаилбоксполици</span><span class="sxs-lookup"><span data-stu-id="c495f-130">exchangeMailboxPolicy</span></span>|<span data-ttu-id="c495f-131">6 </span><span class="sxs-lookup"><span data-stu-id="c495f-131">6</span></span>|<span data-ttu-id="c495f-132">Состояние доступа определяется политикой почтовых ящиков Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-132">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="c495f-133">остальные</span><span class="sxs-lookup"><span data-stu-id="c495f-133">other</span></span>|<span data-ttu-id="c495f-134">7 </span><span class="sxs-lookup"><span data-stu-id="c495f-134">7</span></span>|<span data-ttu-id="c495f-135">Состояние доступа определяется Exchange</span><span class="sxs-lookup"><span data-stu-id="c495f-135">Access state determined by Exchange</span></span>|
|<span data-ttu-id="c495f-136">совместимо</span><span class="sxs-lookup"><span data-stu-id="c495f-136">compliant</span></span>|<span data-ttu-id="c495f-137">8 </span><span class="sxs-lookup"><span data-stu-id="c495f-137">8</span></span>|<span data-ttu-id="c495f-138">Состояние доступа, предоставленное запросом на соответствие</span><span class="sxs-lookup"><span data-stu-id="c495f-138">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="c495f-139">ноткомплиант</span><span class="sxs-lookup"><span data-stu-id="c495f-139">notCompliant</span></span>|<span data-ttu-id="c495f-140">9 </span><span class="sxs-lookup"><span data-stu-id="c495f-140">9</span></span>|<span data-ttu-id="c495f-141">Состояние доступа отозвано с помощью запроса на соответствие</span><span class="sxs-lookup"><span data-stu-id="c495f-141">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="c495f-142">нотенроллед</span><span class="sxs-lookup"><span data-stu-id="c495f-142">notEnrolled</span></span>|<span data-ttu-id="c495f-143">10 </span><span class="sxs-lookup"><span data-stu-id="c495f-143">10</span></span>|<span data-ttu-id="c495f-144">Состояние доступа, аннулированное запросом управления</span><span class="sxs-lookup"><span data-stu-id="c495f-144">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="c495f-145">ункновнлокатион</span><span class="sxs-lookup"><span data-stu-id="c495f-145">unknownLocation</span></span>|<span data-ttu-id="c495f-146">12 </span><span class="sxs-lookup"><span data-stu-id="c495f-146">12</span></span>|<span data-ttu-id="c495f-147">Состояние доступа в связи с неизвестным расположением</span><span class="sxs-lookup"><span data-stu-id="c495f-147">Access state due to unknown location</span></span>|
|<span data-ttu-id="c495f-148">мфарекуиред</span><span class="sxs-lookup"><span data-stu-id="c495f-148">mfaRequired</span></span>|<span data-ttu-id="c495f-149">13 </span><span class="sxs-lookup"><span data-stu-id="c495f-149">13</span></span>|<span data-ttu-id="c495f-150">Состояние доступа из-за вызова MFA</span><span class="sxs-lookup"><span data-stu-id="c495f-150">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="c495f-151">азуреадблоккдуетоакцессполици</span><span class="sxs-lookup"><span data-stu-id="c495f-151">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="c495f-152">14 </span><span class="sxs-lookup"><span data-stu-id="c495f-152">14</span></span>|<span data-ttu-id="c495f-153">Состояние доступа, отозванное политикой доступа AAD</span><span class="sxs-lookup"><span data-stu-id="c495f-153">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="c495f-154">компромиседпассворд</span><span class="sxs-lookup"><span data-stu-id="c495f-154">compromisedPassword</span></span>|<span data-ttu-id="c495f-155">15 </span><span class="sxs-lookup"><span data-stu-id="c495f-155">15</span></span>|<span data-ttu-id="c495f-156">Состояние доступа отозвано с помощью скомпрометированного пароля</span><span class="sxs-lookup"><span data-stu-id="c495f-156">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="c495f-157">девиценоткновнвисманажедапп</span><span class="sxs-lookup"><span data-stu-id="c495f-157">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="c495f-158">16 </span><span class="sxs-lookup"><span data-stu-id="c495f-158">16</span></span>|<span data-ttu-id="c495f-159">Состояние доступа, отозванное с помощью вызова управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="c495f-159">Access state revoked by managed application challenge</span></span>|






