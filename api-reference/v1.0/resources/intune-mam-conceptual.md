---
title: Защита данных корпоративных приложений с помощью Microsoft Intune
description: Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 33e814dc754d564dd3921d7f4369f0112b7a8ec0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732835"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="04e03-103">Защита данных корпоративных приложений с помощью Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="04e03-103">How to protect your company app data with Microsoft Intune</span></span>

<span data-ttu-id="04e03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04e03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04e03-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04e03-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="04e03-106">Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.</span><span class="sxs-lookup"><span data-stu-id="04e03-106">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="04e03-107">Политики защиты приложений в Intune используются для защиты корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="04e03-107">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="04e03-108">Так как эти политики можно использовать вне зависимости от любого решения для управления мобильными устройствами (MDM), защита корпоративных данных обеспечивается как с регистрацией устройства в решении по управлению устройствами, так и без нее.</span><span class="sxs-lookup"><span data-stu-id="04e03-108">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="04e03-109">Внедрив политики уровня приложения, вы можете ограничить доступ к корпоративным ресурсам и оставить данные в поле зрения ИТ-отдела.</span><span class="sxs-lookup"><span data-stu-id="04e03-109">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="04e03-110">Для управления политиками защиты приложений в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="04e03-110">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="04e03-111">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="04e03-111">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="04e03-112">Регистрация управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="04e03-112">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="04e03-113">Идентификатор мобильных приложений для Android</span><span class="sxs-lookup"><span data-stu-id="04e03-113">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="04e03-114">Тип приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-114">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="04e03-115">Защита управляемых приложений по умолчанию</span><span class="sxs-lookup"><span data-stu-id="04e03-115">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="04e03-116">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="04e03-116">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="04e03-117">Регистрация управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="04e03-117">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="04e03-118">Идентификатор мобильных приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="04e03-118">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="04e03-119">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="04e03-119">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="04e03-120">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="04e03-120">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="04e03-121">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="04e03-121">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="04e03-122">JSON</span><span class="sxs-lookup"><span data-stu-id="04e03-122">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="04e03-123">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="04e03-123">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="04e03-124">Уровень совместного доступа к буферу обмена управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-124">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="04e03-125">Конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-125">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="04e03-126">Тип шифрования данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-126">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="04e03-127">Место хранения данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-127">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="04e03-128">Уровень передачи данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-128">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="04e03-129">Состояние диагностики управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-129">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="04e03-130">Причина пометки управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-130">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="04e03-131">Операция управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-131">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="04e03-132">Набор символов ПИН-кода управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="04e03-132">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="04e03-133">Политика управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-133">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="04e03-134">Сводка по развертыванию политик для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-134">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="04e03-135">Сводка по развертыванию политик для отдельных управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-135">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="04e03-136">Защита управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-136">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="04e03-137">Регистрация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-137">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="04e03-138">Состояние управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-138">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="04e03-139">Необработанные данные о состоянии управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-139">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="04e03-140">Управляемое мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="04e03-140">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="04e03-141">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="04e03-141">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="04e03-142">Идентификатор мобильных приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-142">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="04e03-143">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="04e03-143">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="04e03-144">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-144">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="04e03-145">Назначение целевой политики для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-145">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="04e03-146">Целевая защита управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="04e03-146">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="04e03-147">Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-147">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="04e03-148">Приложение Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-148">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="04e03-149">Сводка по обучению приложения Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-149">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="04e03-150">Файл AppLocker для Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-150">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="04e03-151">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-151">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="04e03-152">Классическое приложение Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-152">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="04e03-153">Уровень применения Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-153">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="04e03-154">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-154">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="04e03-155">Сводка по обучению сети Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-155">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="04e03-156">Требования к символам ПИН-кода Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-156">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="04e03-157">Политика Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-157">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="04e03-158">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-158">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="04e03-159">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-159">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="04e03-160">Приложение из магазина Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="04e03-160">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)






