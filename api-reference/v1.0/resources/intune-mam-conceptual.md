---
title: Защита данных корпоративных приложений с помощью Microsoft Intune
description: Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 5f655e8b80a2f07164a8560146e1f1e2d4c1f7ec
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356557"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="fe6b6-103">Защита данных корпоративных приложений с помощью Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fe6b6-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="fe6b6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe6b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="fe6b6-105">Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.</span><span class="sxs-lookup"><span data-stu-id="fe6b6-105">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="fe6b6-106">Политики защиты приложений в Intune используются для защиты корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="fe6b6-106">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="fe6b6-107">Так как эти политики можно использовать вне зависимости от любого решения для управления мобильными устройствами (MDM), защита корпоративных данных обеспечивается как с регистрацией устройства в решении по управлению устройствами, так и без нее.</span><span class="sxs-lookup"><span data-stu-id="fe6b6-107">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="fe6b6-108">Внедрив политики уровня приложения, вы можете ограничить доступ к корпоративным ресурсам и оставить данные в поле зрения ИТ-отдела.</span><span class="sxs-lookup"><span data-stu-id="fe6b6-108">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="fe6b6-109">Для управления политиками защиты приложений в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="fe6b6-109">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="fe6b6-110">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="fe6b6-110">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="fe6b6-111">Регистрация управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="fe6b6-111">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="fe6b6-112">Идентификатор мобильных приложений для Android</span><span class="sxs-lookup"><span data-stu-id="fe6b6-112">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="fe6b6-113">Тип приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-113">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="fe6b6-114">Защита управляемых приложений по умолчанию</span><span class="sxs-lookup"><span data-stu-id="fe6b6-114">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="fe6b6-115">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="fe6b6-115">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="fe6b6-116">Регистрация управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="fe6b6-116">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="fe6b6-117">Идентификатор мобильных приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="fe6b6-117">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="fe6b6-118">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="fe6b6-118">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="fe6b6-119">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="fe6b6-119">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="fe6b6-120">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="fe6b6-120">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="fe6b6-121">JSON</span><span class="sxs-lookup"><span data-stu-id="fe6b6-121">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="fe6b6-122">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="fe6b6-122">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="fe6b6-123">Уровень совместного доступа к буферу обмена управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="fe6b6-124">Конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="fe6b6-125">Тип шифрования данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="fe6b6-126">Место хранения данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="fe6b6-127">Уровень передачи данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="fe6b6-128">Состояние диагностики управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="fe6b6-129">Причина пометки управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="fe6b6-130">Операция управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="fe6b6-131">Набор символов ПИН-кода управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="fe6b6-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="fe6b6-132">Политика управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="fe6b6-133">Сводка по развертыванию политик для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="fe6b6-134">Сводка по развертыванию политик для отдельных управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="fe6b6-135">Защита управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="fe6b6-136">Регистрация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="fe6b6-137">Состояние управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-137">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="fe6b6-138">Необработанные данные о состоянии управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-138">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="fe6b6-139">Управляемое мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="fe6b6-139">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="fe6b6-140">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="fe6b6-140">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="fe6b6-141">Идентификатор мобильных приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-141">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="fe6b6-142">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="fe6b6-142">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="fe6b6-143">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="fe6b6-144">Назначение целевой политики для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="fe6b6-145">Целевая защита управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="fe6b6-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="fe6b6-146">Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="fe6b6-147">Приложение Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="fe6b6-148">Сводка по обучению приложения Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="fe6b6-149">Файл AppLocker для Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="fe6b6-150">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="fe6b6-151">Классическое приложение Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="fe6b6-152">Уровень применения Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="fe6b6-153">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="fe6b6-154">Сводка по обучению сети Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="fe6b6-155">Требования к символам ПИН-кода Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="fe6b6-156">Политика Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="fe6b6-157">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="fe6b6-158">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="fe6b6-159">Приложение из магазина Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6b6-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)

