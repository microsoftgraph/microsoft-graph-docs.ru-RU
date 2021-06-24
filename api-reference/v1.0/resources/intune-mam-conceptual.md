---
title: Защита данных корпоративных приложений с помощью Microsoft Intune
description: Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 50630540984b917e063eab65b6878370ea414d61
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108805"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="81657-103">Защита данных корпоративных приложений с помощью Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="81657-103">How to protect your company app data with Microsoft Intune</span></span>

<span data-ttu-id="81657-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81657-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81657-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="81657-106">Политики защиты приложений в Microsoft Intune помогают защитить корпоративные данные и предотвратить потерю данных.</span><span class="sxs-lookup"><span data-stu-id="81657-106">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="81657-107">Политики защиты приложений в Intune используются для защиты корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="81657-107">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="81657-108">Так как эти политики можно использовать вне зависимости от любого решения для управления мобильными устройствами (MDM), защита корпоративных данных обеспечивается как с регистрацией устройства в решении по управлению устройствами, так и без нее.</span><span class="sxs-lookup"><span data-stu-id="81657-108">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="81657-109">Внедрив политики уровня приложения, вы можете ограничить доступ к корпоративным ресурсам и оставить данные в поле зрения ИТ-отдела.</span><span class="sxs-lookup"><span data-stu-id="81657-109">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="81657-110">Для управления политиками защиты приложений в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="81657-110">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="81657-111">Защита управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="81657-111">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="81657-112">Регистрация управляемых приложений для Android</span><span class="sxs-lookup"><span data-stu-id="81657-112">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="81657-113">Идентификатор мобильных приложений для Android</span><span class="sxs-lookup"><span data-stu-id="81657-113">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="81657-114">Тип приложения</span><span class="sxs-lookup"><span data-stu-id="81657-114">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="81657-115">Защита управляемых приложений по умолчанию</span><span class="sxs-lookup"><span data-stu-id="81657-115">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="81657-116">Управление приложениями для устройств</span><span class="sxs-lookup"><span data-stu-id="81657-116">Device app management</span></span>](intune-mam-deviceappmanagement.md)
- [<span data-ttu-id="81657-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="81657-117">Device management</span></span>](intune-wip-devicemanagement.md)
- [<span data-ttu-id="81657-118">Защита управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="81657-118">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="81657-119">Регистрация управляемых приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="81657-119">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="81657-120">Идентификатор мобильных приложений для iOS</span><span class="sxs-lookup"><span data-stu-id="81657-120">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="81657-121">Диапазон IP-адресов</span><span class="sxs-lookup"><span data-stu-id="81657-121">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="81657-122">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="81657-122">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="81657-123">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="81657-123">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="81657-124">JSON</span><span class="sxs-lookup"><span data-stu-id="81657-124">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="81657-125">Пара "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="81657-125">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="81657-126">Уровень совместного доступа к буферу обмена управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="81657-126">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="81657-127">Конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-127">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="81657-128">Тип шифрования данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="81657-128">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="81657-129">Место хранения данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="81657-129">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="81657-130">Уровень передачи данных управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="81657-130">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="81657-131">Состояние диагностики управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-131">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="81657-132">Причина пометки управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="81657-132">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="81657-133">Операция управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-133">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="81657-134">Набор символов ПИН-кода управляемого приложения</span><span class="sxs-lookup"><span data-stu-id="81657-134">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="81657-135">Политика управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-135">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="81657-136">Сводка по развертыванию политик для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-136">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="81657-137">Сводка по развертыванию политик для отдельных управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-137">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="81657-138">Защита управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-138">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="81657-139">Регистрация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-139">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="81657-140">Состояние управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-140">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="81657-141">Необработанные данные о состоянии управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-141">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="81657-142">Тип управляемого браузера</span><span class="sxs-lookup"><span data-stu-id="81657-142">Managed browser type</span></span>](intune-mam-managedbrowsertype.md)
- [<span data-ttu-id="81657-143">Управляемое мобильное приложение</span><span class="sxs-lookup"><span data-stu-id="81657-143">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="81657-144">Политика Windows Information Protection для MDM</span><span class="sxs-lookup"><span data-stu-id="81657-144">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="81657-145">Идентификатор мобильных приложений</span><span class="sxs-lookup"><span data-stu-id="81657-145">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="81657-146">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="81657-146">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="81657-147">Целевая конфигурация управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-147">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="81657-148">Назначение целевой политики для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-148">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="81657-149">Целевая защита управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="81657-149">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="81657-150">Пользователь</span><span class="sxs-lookup"><span data-stu-id="81657-150">User</span></span>](intune-mam-user.md)
- [<span data-ttu-id="81657-151">Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-151">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="81657-152">Приложение Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-152">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="81657-153">Сводка по обучению приложения Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-153">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="81657-154">Файл AppLocker для Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-154">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="81657-155">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-155">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="81657-156">Классическое приложение Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-156">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="81657-157">Уровень применения Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-157">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="81657-158">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-158">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="81657-159">Сводка по обучению сети Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-159">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="81657-160">Требования к символам ПИН-кода Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-160">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="81657-161">Политика Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-161">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="81657-162">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-162">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="81657-163">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-163">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="81657-164">Приложение из магазина Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="81657-164">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)