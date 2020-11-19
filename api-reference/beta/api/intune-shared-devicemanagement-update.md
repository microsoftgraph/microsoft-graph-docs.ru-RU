---
title: Обновление объекта deviceManagement
description: Обновление свойств объекта deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bf6b5031c53da45af63517e52f03d344f71a4c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210132"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="d64d8-103">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d64d8-103">Update deviceManagement</span></span>

<span data-ttu-id="d64d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d64d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d64d8-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d64d8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d64d8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d64d8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d64d8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d64d8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d64d8-108">Обновление свойств объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d64d8-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d64d8-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d64d8-109">Prerequisites</span></span>

<span data-ttu-id="d64d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d64d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d64d8-112">Обратите внимание, что разрешение зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="d64d8-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="d64d8-113">&nbsp;Тип разрешения &nbsp; (по &nbsp; рабочим процессам)</span><span class="sxs-lookup"><span data-stu-id="d64d8-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="d64d8-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d64d8-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="d64d8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d64d8-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="d64d8-116">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="d64d8-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d64d8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="d64d8-118">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="d64d8-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d64d8-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-120">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="d64d8-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d64d8-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-122">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d64d8-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d64d8-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-124">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="d64d8-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d64d8-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d64d8-126">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d64d8-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d64d8-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-128">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="d64d8-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d64d8-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-130">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d64d8-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d64d8-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-132">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="d64d8-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d64d8-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-134">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="d64d8-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d64d8-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-136">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="d64d8-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="d64d8-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-138">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d64d8-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d64d8-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-140">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d64d8-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d64d8-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-142">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="d64d8-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="d64d8-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-144">&nbsp;&nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="d64d8-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d64d8-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d64d8-146">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="d64d8-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d64d8-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-148">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="d64d8-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="d64d8-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-150">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="d64d8-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d64d8-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-152">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="d64d8-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="d64d8-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-154">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d64d8-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d64d8-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-156">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d64d8-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d64d8-157">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d64d8-157">Not supported.</span></span>|
| <span data-ttu-id="d64d8-158">Приложение</span><span class="sxs-lookup"><span data-stu-id="d64d8-158">Application</span></span> ||
| <span data-ttu-id="d64d8-159">&nbsp;&nbsp; **Android для работы**</span><span class="sxs-lookup"><span data-stu-id="d64d8-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d64d8-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="d64d8-161">&nbsp; &nbsp; **Аудит**</span><span class="sxs-lookup"><span data-stu-id="d64d8-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d64d8-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-163">&nbsp; &nbsp; **Условия компании**</span><span class="sxs-lookup"><span data-stu-id="d64d8-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d64d8-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-165">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="d64d8-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d64d8-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-167">&nbsp;&nbsp; **Цель устройства**</span><span class="sxs-lookup"><span data-stu-id="d64d8-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d64d8-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d64d8-169">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d64d8-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d64d8-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-171">&nbsp;&nbsp; **Электронная SIM-карта**</span><span class="sxs-lookup"><span data-stu-id="d64d8-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d64d8-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-173">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="d64d8-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d64d8-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-175">&nbsp;&nbsp; **Ограждение**</span><span class="sxs-lookup"><span data-stu-id="d64d8-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d64d8-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-177">&nbsp; &nbsp; **Уведомление**</span><span class="sxs-lookup"><span data-stu-id="d64d8-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d64d8-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-179">&nbsp;&nbsp; **Одж**</span><span class="sxs-lookup"><span data-stu-id="d64d8-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="d64d8-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-181">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d64d8-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d64d8-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-183">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d64d8-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d64d8-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-185">&nbsp; &nbsp; **Управление доступом на основе ролей (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="d64d8-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="d64d8-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-187">&nbsp;&nbsp; **Удаленный доступ**</span><span class="sxs-lookup"><span data-stu-id="d64d8-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d64d8-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d64d8-189">&nbsp;&nbsp; **Удаленная помощь**</span><span class="sxs-lookup"><span data-stu-id="d64d8-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d64d8-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-191">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="d64d8-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="d64d8-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-193">&nbsp;&nbsp; **Управление расходами по телекоммуникационной** связи</span><span class="sxs-lookup"><span data-stu-id="d64d8-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d64d8-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-195">&nbsp;&nbsp; **Траублехутинг**</span><span class="sxs-lookup"><span data-stu-id="d64d8-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="d64d8-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d64d8-197">&nbsp; &nbsp; **Windows Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d64d8-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d64d8-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64d8-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d64d8-199">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d64d8-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="d64d8-200">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d64d8-200">Request headers</span></span>

|<span data-ttu-id="d64d8-201">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d64d8-201">Header</span></span>|<span data-ttu-id="d64d8-202">Значение</span><span class="sxs-lookup"><span data-stu-id="d64d8-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d64d8-203">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d64d8-203">Authorization</span></span>|<span data-ttu-id="d64d8-204">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d64d8-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d64d8-205">Accept</span><span class="sxs-lookup"><span data-stu-id="d64d8-205">Accept</span></span>|<span data-ttu-id="d64d8-206">application/json</span><span class="sxs-lookup"><span data-stu-id="d64d8-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d64d8-207">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d64d8-207">Request body</span></span>

<span data-ttu-id="d64d8-208">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune-shared-devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d64d8-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="d64d8-209">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="d64d8-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="d64d8-210">Свойство</span><span class="sxs-lookup"><span data-stu-id="d64d8-210">Property</span></span>|<span data-ttu-id="d64d8-211">Тип</span><span class="sxs-lookup"><span data-stu-id="d64d8-211">Type</span></span>|<span data-ttu-id="d64d8-212">Описание</span><span class="sxs-lookup"><span data-stu-id="d64d8-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d64d8-213">id</span><span class="sxs-lookup"><span data-stu-id="d64d8-213">id</span></span>|<span data-ttu-id="d64d8-214">String</span><span class="sxs-lookup"><span data-stu-id="d64d8-214">String</span></span>|<span data-ttu-id="d64d8-215">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="d64d8-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="d64d8-216">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="d64d8-216">**Device configuration**</span></span>|
|<span data-ttu-id="d64d8-217">интунеаккаунтид</span><span class="sxs-lookup"><span data-stu-id="d64d8-217">intuneAccountId</span></span>|<span data-ttu-id="d64d8-218">GUID</span><span class="sxs-lookup"><span data-stu-id="d64d8-218">GUID</span></span>|<span data-ttu-id="d64d8-219">Идентификатор учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="d64d8-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="d64d8-220">легаципкмананжементенаблед</span><span class="sxs-lookup"><span data-stu-id="d64d8-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="d64d8-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64d8-221">Boolean</span></span>|<span data-ttu-id="d64d8-222">Свойство, позволяющее управлять устаревшим управлением устаревших ПК для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d64d8-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="d64d8-223">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d64d8-223">This property is read-only.</span></span>|
|<span data-ttu-id="d64d8-224">максимумдептокенс</span><span class="sxs-lookup"><span data-stu-id="d64d8-224">maximumDepTokens</span></span>|<span data-ttu-id="d64d8-225">Int32</span><span class="sxs-lookup"><span data-stu-id="d64d8-225">Int32</span></span>|<span data-ttu-id="d64d8-226">Максимальное число маркеров DEP, разрешенных для каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="d64d8-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="d64d8-227">settings</span><span class="sxs-lookup"><span data-stu-id="d64d8-227">settings</span></span>|[<span data-ttu-id="d64d8-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="d64d8-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="d64d8-229">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d64d8-229">Account level settings.</span></span>|
|<span data-ttu-id="d64d8-230">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d64d8-230">**Device management**</span></span>|
|<span data-ttu-id="d64d8-231">аккаунтмовекомплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="d64d8-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="d64d8-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d64d8-232">DateTimeOffset</span></span>|<span data-ttu-id="d64d8-233">Дата & время, когда данные клиента перемещаются между скалеунитс.</span><span class="sxs-lookup"><span data-stu-id="d64d8-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="d64d8-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="d64d8-234">adminConsent</span></span>|[<span data-ttu-id="d64d8-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="d64d8-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="d64d8-236">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="d64d8-236">Admin consent information.</span></span>|
|<span data-ttu-id="d64d8-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="d64d8-237">deviceProtectionOverview</span></span>|<span data-ttu-id="d64d8-238">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md);</span><span class="sxs-lookup"><span data-stu-id="d64d8-238">[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)</span></span>|<span data-ttu-id="d64d8-239">Общие сведения о защите устройств.</span><span class="sxs-lookup"><span data-stu-id="d64d8-239">Device protection overview.</span></span>|
|<span data-ttu-id="d64d8-240">managedDeviceCleanupSettings;</span><span class="sxs-lookup"><span data-stu-id="d64d8-240">managedDeviceCleanupSettings</span></span>|<span data-ttu-id="d64d8-241">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md);</span><span class="sxs-lookup"><span data-stu-id="d64d8-241">[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)</span></span>|<span data-ttu-id="d64d8-242">Правило очистки устройств</span><span class="sxs-lookup"><span data-stu-id="d64d8-242">Device cleanup rule</span></span>|
|<span data-ttu-id="d64d8-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="d64d8-243">subscriptionState</span></span>|[<span data-ttu-id="d64d8-244">девицеманажементсубскриптионстате</span><span class="sxs-lookup"><span data-stu-id="d64d8-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="d64d8-245">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="d64d8-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="d64d8-246">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="d64d8-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="d64d8-247">subscriptions</span><span class="sxs-lookup"><span data-stu-id="d64d8-247">subscriptions</span></span>|[<span data-ttu-id="d64d8-248">девицеманажементсубскриптионс</span><span class="sxs-lookup"><span data-stu-id="d64d8-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="d64d8-249">Подписка клиента.</span><span class="sxs-lookup"><span data-stu-id="d64d8-249">Tenant's Subscription.</span></span> <span data-ttu-id="d64d8-250">Возможные значения: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="d64d8-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="d64d8-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="d64d8-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="d64d8-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="d64d8-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="d64d8-253">Обзор вредоносных программ для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="d64d8-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="d64d8-254">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d64d8-254">**Onboarding**</span></span>|
|<span data-ttu-id="d64d8-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="d64d8-255">intuneBrand</span></span>|[<span data-ttu-id="d64d8-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="d64d8-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="d64d8-257">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="d64d8-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="d64d8-258">Поддержка свойств текста запроса зависит от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="d64d8-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="d64d8-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="d64d8-259">Response</span></span>
<span data-ttu-id="d64d8-260">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune-shared-devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d64d8-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d64d8-261">Пример</span><span class="sxs-lookup"><span data-stu-id="d64d8-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="d64d8-262">Запрос</span><span class="sxs-lookup"><span data-stu-id="d64d8-262">Request</span></span>

<span data-ttu-id="d64d8-263">Ниже приведен пример запроса, который следует за рабочим процессом управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="d64d8-263">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="d64d8-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="d64d8-264">Response</span></span>

<span data-ttu-id="d64d8-265">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d64d8-265">Here is an example of the response.</span></span> 

<span data-ttu-id="d64d8-266">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d64d8-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d64d8-267">Возвращаемые свойства различаются в зависимости от рабочего процесса и контекста.</span><span class="sxs-lookup"><span data-stu-id="d64d8-267">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```










