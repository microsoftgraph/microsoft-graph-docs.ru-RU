---
title: Получение deviceManagement
description: Чтение свойств и связей объекта deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 89fbc5f549b86838eace46e4d5a0c182d6b3a44d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086076"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="69680-103">Получение deviceManagement</span><span class="sxs-lookup"><span data-stu-id="69680-103">Get deviceManagement</span></span>

> <span data-ttu-id="69680-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="69680-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69680-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69680-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69680-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69680-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69680-107">Чтение свойств и связей объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="69680-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69680-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69680-108">Prerequisites</span></span>

<span data-ttu-id="69680-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69680-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69680-111">Тип&nbsp;&nbsp;разрешения (по&nbsp;рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="69680-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="69680-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69680-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="69680-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69680-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="69680-114">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="69680-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="69680-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-116">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="69680-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="69680-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="69680-118">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="69680-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="69680-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="69680-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="69680-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-122">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="69680-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="69680-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="69680-124">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="69680-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="69680-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="69680-126">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="69680-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="69680-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-128">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="69680-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="69680-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-130">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="69680-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="69680-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-132">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="69680-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="69680-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-134">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="69680-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="69680-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-136">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="69680-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="69680-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-138">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="69680-138">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="69680-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-140">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="69680-140">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="69680-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="69680-142">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="69680-142">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="69680-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-144">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="69680-144">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="69680-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-146">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="69680-146">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="69680-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-148">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="69680-148">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="69680-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-150">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="69680-150">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="69680-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="69680-152">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="69680-152">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="69680-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="69680-154">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69680-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69680-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69680-155">Not supported.</span></span>|
| <span data-ttu-id="69680-156">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69680-156">Application</span></span> | |
| <span data-ttu-id="69680-157">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="69680-157">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="69680-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-159">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="69680-159">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="69680-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="69680-161">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="69680-161">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="69680-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-163">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="69680-163">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="69680-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-165">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="69680-165">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="69680-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="69680-167">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="69680-167">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="69680-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="69680-169">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="69680-169">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="69680-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-171">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="69680-171">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="69680-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-173">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="69680-173">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="69680-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-175">&nbsp;&nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="69680-175">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="69680-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-177">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="69680-177">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="69680-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-179">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="69680-179">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="69680-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-181">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="69680-181">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="69680-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-183">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="69680-183">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="69680-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="69680-185">&nbsp; &nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="69680-185">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="69680-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="69680-187">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="69680-187">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="69680-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-189">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="69680-189">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="69680-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-191">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="69680-191">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="69680-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="69680-193">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="69680-193">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="69680-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="69680-195">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="69680-195">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="69680-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69680-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69680-197">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69680-197">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69680-198">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69680-198">Optional query parameters</span></span>

<span data-ttu-id="69680-199">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="69680-199">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69680-200">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69680-200">Request headers</span></span>
|<span data-ttu-id="69680-201">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69680-201">Header</span></span>|<span data-ttu-id="69680-202">Значение</span><span class="sxs-lookup"><span data-stu-id="69680-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69680-203">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69680-203">Authorization</span></span>|<span data-ttu-id="69680-204">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69680-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69680-205">Accept</span><span class="sxs-lookup"><span data-stu-id="69680-205">Accept</span></span>|<span data-ttu-id="69680-206">application/json</span><span class="sxs-lookup"><span data-stu-id="69680-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69680-207">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69680-207">Request body</span></span>

<span data-ttu-id="69680-208">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69680-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69680-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="69680-209">Response</span></span>

<span data-ttu-id="69680-210">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="69680-210">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69680-211">Пример</span><span class="sxs-lookup"><span data-stu-id="69680-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="69680-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="69680-212">Request</span></span>

<span data-ttu-id="69680-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69680-213">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="69680-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="69680-214">Response</span></span>

<span data-ttu-id="69680-215">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="69680-215">Here are example of the response.</span></span> 

<span data-ttu-id="69680-216">Note: объекты ответа, показанные здесь, могут быть усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="69680-216">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="69680-217">Возвращаются свойства, подходящие для рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="69680-217">Properties appropriate for the workflow are returned.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```












