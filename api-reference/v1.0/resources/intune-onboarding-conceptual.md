---
title: Регистрация устройств для управления в Intune
description: " (BYOD) регистрация позволяет пользователям регистрировать личные телефоны, Планшетные ПК или ПК. Регистрация по программе \"Корпоративное устройство\" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства."
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 54a2a8bb3901f1a6938401963e8efcbd9e02f194
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360589"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="3f1aa-104">Регистрация устройств для управления в Intune</span><span class="sxs-lookup"><span data-stu-id="3f1aa-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="3f1aa-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="3f1aa-106">Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-106">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="3f1aa-107">В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-107">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="3f1aa-108">Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-108">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="3f1aa-109">По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-109">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="3f1aa-110">Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-110">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="3f1aa-111">Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="3f1aa-111">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="3f1aa-112">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="3f1aa-112">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="3f1aa-113">Настройка ограничения регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="3f1aa-113">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="3f1aa-114">Ограничение платформы для регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="3f1aa-114">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="3f1aa-115">Настройка ограничений для платформы регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="3f1aa-115">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="3f1aa-116">Настройка регистрации устройств в Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="3f1aa-116">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="3f1aa-117">Соединитель Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-117">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="3f1aa-118">Состояние соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-118">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="3f1aa-119">Тип синхронизации соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-119">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="3f1aa-120">Тип соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-120">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="3f1aa-121">Партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-121">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="3f1aa-122">Тип партнерского приложения для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-122">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="3f1aa-123">Состояние клиента партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="3f1aa-123">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="3f1aa-124">Включение</span><span class="sxs-lookup"><span data-stu-id="3f1aa-124">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="3f1aa-125">Назначение конфигураций регистрации</span><span class="sxs-lookup"><span data-stu-id="3f1aa-125">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="3f1aa-126">Торговая марка Intune</span><span class="sxs-lookup"><span data-stu-id="3f1aa-126">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="3f1aa-127">Центр MDM</span><span class="sxs-lookup"><span data-stu-id="3f1aa-127">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="3f1aa-128">Соединитель Mobile Threat Defense</span><span class="sxs-lookup"><span data-stu-id="3f1aa-128">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="3f1aa-129">Состояние клиента партнера Mobile Threat Defense</span><span class="sxs-lookup"><span data-stu-id="3f1aa-129">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="3f1aa-130">Настройка локального условного доступа</span><span class="sxs-lookup"><span data-stu-id="3f1aa-130">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="3f1aa-131">Организация</span><span class="sxs-lookup"><span data-stu-id="3f1aa-131">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="3f1aa-132">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="3f1aa-132">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="3f1aa-133">Маркер VPP</span><span class="sxs-lookup"><span data-stu-id="3f1aa-133">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="3f1aa-134">Состояние токена VPP</span><span class="sxs-lookup"><span data-stu-id="3f1aa-134">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="3f1aa-135">Состояние синхронизации токена VPP</span><span class="sxs-lookup"><span data-stu-id="3f1aa-135">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="3f1aa-136">Использование ПИН-кода в Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="3f1aa-136">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)

