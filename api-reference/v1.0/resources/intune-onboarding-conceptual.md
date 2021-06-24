---
title: Регистрация устройств для управления в Intune
description: " (BYOD) регистрация позволяет пользователям записать свои личные телефоны, планшеты или компьютеры. Регистрация по программе \"Корпоративное устройство\" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства."
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: d8a68ee75a267da062a462c8f015f1832494c5e1
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107748"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="8761c-104">Регистрация устройств для управления в Intune</span><span class="sxs-lookup"><span data-stu-id="8761c-104">Enroll devices for management in Intune</span></span>

<span data-ttu-id="8761c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8761c-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8761c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8761c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="8761c-107">Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8761c-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="8761c-108">В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune.</span><span class="sxs-lookup"><span data-stu-id="8761c-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="8761c-109">Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления.</span><span class="sxs-lookup"><span data-stu-id="8761c-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="8761c-110">По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры.</span><span class="sxs-lookup"><span data-stu-id="8761c-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="8761c-111">Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.</span><span class="sxs-lookup"><span data-stu-id="8761c-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="8761c-112">Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="8761c-112">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="8761c-113">Партнер по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="8761c-113">Compliance management partner</span></span>](intune-onboarding-compliancemanagementpartner.md)
- [<span data-ttu-id="8761c-114">Назначение партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="8761c-114">Compliance management partner assignment</span></span>](intune-onboarding-compliancemanagementpartnerassignment.md)
- [<span data-ttu-id="8761c-115">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="8761c-115">Device app management</span></span>](intune-onboarding-deviceappmanagement.md)
- [<span data-ttu-id="8761c-116">Категория устройств</span><span class="sxs-lookup"><span data-stu-id="8761c-116">Device category</span></span>](intune-onboarding-devicecategory.md)
- [<span data-ttu-id="8761c-117">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="8761c-117">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="8761c-118">Настройка ограничения регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="8761c-118">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="8761c-119">Ограничение платформы для регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="8761c-119">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="8761c-120">Настройка ограничений для платформы регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="8761c-120">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="8761c-121">Настройка регистрации устройств в Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="8761c-121">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="8761c-122">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-122">Device management</span></span>](intune-onboarding-devicemanagement.md)
- [<span data-ttu-id="8761c-123">Соединитель Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-123">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="8761c-124">Состояние соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-124">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="8761c-125">Тип синхронизации соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-125">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="8761c-126">Тип соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-126">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="8761c-127">Партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-127">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="8761c-128">Тип партнерского приложения для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-128">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="8761c-129">Состояние клиента партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="8761c-129">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="8761c-130">Включение</span><span class="sxs-lookup"><span data-stu-id="8761c-130">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="8761c-131">Назначение конфигураций регистрации</span><span class="sxs-lookup"><span data-stu-id="8761c-131">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="8761c-132">Торговая марка Intune</span><span class="sxs-lookup"><span data-stu-id="8761c-132">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="8761c-133">Центр MDM</span><span class="sxs-lookup"><span data-stu-id="8761c-133">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="8761c-134">Соединитель Mobile Threat Defense</span><span class="sxs-lookup"><span data-stu-id="8761c-134">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="8761c-135">Состояние клиента партнера Mobile Threat Defense</span><span class="sxs-lookup"><span data-stu-id="8761c-135">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="8761c-136">Настройка локального условного доступа</span><span class="sxs-lookup"><span data-stu-id="8761c-136">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="8761c-137">Организация</span><span class="sxs-lookup"><span data-stu-id="8761c-137">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="8761c-138">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="8761c-138">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="8761c-139">Пользователь</span><span class="sxs-lookup"><span data-stu-id="8761c-139">User</span></span>](intune-onboarding-user.md)
- [<span data-ttu-id="8761c-140">Маркер VPP</span><span class="sxs-lookup"><span data-stu-id="8761c-140">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="8761c-141">Состояние токена VPP</span><span class="sxs-lookup"><span data-stu-id="8761c-141">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="8761c-142">Состояние синхронизации токена VPP</span><span class="sxs-lookup"><span data-stu-id="8761c-142">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="8761c-143">Использование ПИН-кода в Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="8761c-143">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)