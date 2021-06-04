---
title: Регистрация устройств для управления в Intune
description: " (BYOD) регистрация позволяет пользователям записать свои личные телефоны, планшеты или компьютеры. Регистрация по программе \"Корпоративное устройство\" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства."
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7307e0bc710fead998260e78d0b4f550cffa5b3e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732944"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="fccf0-104">Регистрация устройств для управления в Intune</span><span class="sxs-lookup"><span data-stu-id="fccf0-104">Enroll devices for management in Intune</span></span>

<span data-ttu-id="fccf0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fccf0-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fccf0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fccf0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="fccf0-107">Вы можете зарегистрировать устройства, в том числе компьютеры с Windows, включив управление мобильными устройствами (MDM) с помощью Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="fccf0-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="fccf0-108">В этой статье описано несколько способов регистрации мобильных устройств для управления в Intune.</span><span class="sxs-lookup"><span data-stu-id="fccf0-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="fccf0-109">Способ регистрации устройств зависит от типа устройства, его владельца и необходимого уровня управления.</span><span class="sxs-lookup"><span data-stu-id="fccf0-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="fccf0-110">По программе "принеси свое устройство" (BYOD) пользователи могут зарегистрировать личные телефоны, планшеты или компьютеры.</span><span class="sxs-lookup"><span data-stu-id="fccf0-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="fccf0-111">Регистрация по программе "Корпоративное устройство" (COD) обеспечивает такие сценарии управления, как удаленная очистка, использование общих устройств или сходство пользователя для устройства.</span><span class="sxs-lookup"><span data-stu-id="fccf0-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="fccf0-112">Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="fccf0-112">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="fccf0-113">Настройка регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="fccf0-113">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="fccf0-114">Настройка ограничения регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="fccf0-114">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="fccf0-115">Ограничение платформы для регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="fccf0-115">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="fccf0-116">Настройка ограничений для платформы регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="fccf0-116">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="fccf0-117">Настройка регистрации устройств в Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="fccf0-117">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="fccf0-118">Соединитель Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-118">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="fccf0-119">Состояние соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-119">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="fccf0-120">Тип синхронизации соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-120">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="fccf0-121">Тип соединителя Exchange для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-121">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="fccf0-122">Партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-122">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="fccf0-123">Тип партнерского приложения для управления устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-123">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="fccf0-124">Состояние клиента партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="fccf0-124">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="fccf0-125">Включение</span><span class="sxs-lookup"><span data-stu-id="fccf0-125">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="fccf0-126">Назначение конфигураций регистрации</span><span class="sxs-lookup"><span data-stu-id="fccf0-126">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="fccf0-127">Торговая марка Intune</span><span class="sxs-lookup"><span data-stu-id="fccf0-127">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="fccf0-128">Центр MDM</span><span class="sxs-lookup"><span data-stu-id="fccf0-128">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="fccf0-129">Соединитель Mobile Threat Defense</span><span class="sxs-lookup"><span data-stu-id="fccf0-129">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="fccf0-130">Состояние клиента партнера Mobile Threat Defense</span><span class="sxs-lookup"><span data-stu-id="fccf0-130">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="fccf0-131">Настройка локального условного доступа</span><span class="sxs-lookup"><span data-stu-id="fccf0-131">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="fccf0-132">Организация</span><span class="sxs-lookup"><span data-stu-id="fccf0-132">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="fccf0-133">Цвет RGB</span><span class="sxs-lookup"><span data-stu-id="fccf0-133">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="fccf0-134">Маркер VPP</span><span class="sxs-lookup"><span data-stu-id="fccf0-134">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="fccf0-135">Состояние токена VPP</span><span class="sxs-lookup"><span data-stu-id="fccf0-135">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="fccf0-136">Состояние синхронизации токена VPP</span><span class="sxs-lookup"><span data-stu-id="fccf0-136">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="fccf0-137">Использование ПИН-кода в Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="fccf0-137">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)






