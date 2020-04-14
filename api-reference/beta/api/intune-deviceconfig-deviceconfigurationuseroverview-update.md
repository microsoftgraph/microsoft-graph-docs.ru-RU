---
title: Обновление объекта deviceConfigurationUserOverview
description: Обновление свойств объекта deviceConfigurationUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b2b275aacc807d45918fe0f058a0cc8f5559967
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433303"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="55290-103">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="55290-103">Update deviceConfigurationUserOverview</span></span>

<span data-ttu-id="55290-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55290-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55290-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55290-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55290-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55290-107">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="55290-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55290-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55290-108">Prerequisites</span></span>
<span data-ttu-id="55290-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55290-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55290-111">Permission type</span></span>|<span data-ttu-id="55290-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55290-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55290-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55290-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55290-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55290-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55290-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55290-116">Not supported.</span></span>|
|<span data-ttu-id="55290-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="55290-117">Application</span></span>|<span data-ttu-id="55290-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55290-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55290-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55290-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="55290-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55290-120">Request headers</span></span>
|<span data-ttu-id="55290-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55290-121">Header</span></span>|<span data-ttu-id="55290-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55290-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55290-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55290-123">Authorization</span></span>|<span data-ttu-id="55290-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55290-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55290-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55290-125">Accept</span></span>|<span data-ttu-id="55290-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55290-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55290-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55290-127">Request body</span></span>
<span data-ttu-id="55290-128">В тексте запроса добавьте представление объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55290-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="55290-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="55290-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="55290-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55290-130">Property</span></span>|<span data-ttu-id="55290-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55290-131">Type</span></span>|<span data-ttu-id="55290-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55290-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55290-133">id</span><span class="sxs-lookup"><span data-stu-id="55290-133">id</span></span>|<span data-ttu-id="55290-134">String</span><span class="sxs-lookup"><span data-stu-id="55290-134">String</span></span>|<span data-ttu-id="55290-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55290-135">Key of the entity.</span></span>|
|<span data-ttu-id="55290-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="55290-136">pendingCount</span></span>|<span data-ttu-id="55290-137">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-137">Int32</span></span>|<span data-ttu-id="55290-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="55290-138">Number of pending Users</span></span>|
|<span data-ttu-id="55290-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="55290-139">notApplicableCount</span></span>|<span data-ttu-id="55290-140">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-140">Int32</span></span>|<span data-ttu-id="55290-141">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="55290-141">Number of not applicable users</span></span>|
|<span data-ttu-id="55290-142">successCount</span><span class="sxs-lookup"><span data-stu-id="55290-142">successCount</span></span>|<span data-ttu-id="55290-143">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-143">Int32</span></span>|<span data-ttu-id="55290-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="55290-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="55290-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="55290-145">errorCount</span></span>|<span data-ttu-id="55290-146">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-146">Int32</span></span>|<span data-ttu-id="55290-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="55290-147">Number of error Users</span></span>|
|<span data-ttu-id="55290-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="55290-148">failedCount</span></span>|<span data-ttu-id="55290-149">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-149">Int32</span></span>|<span data-ttu-id="55290-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="55290-150">Number of failed Users</span></span>|
|<span data-ttu-id="55290-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="55290-151">conflictCount</span></span>|<span data-ttu-id="55290-152">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-152">Int32</span></span>|<span data-ttu-id="55290-153">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="55290-153">Number of users in conflict</span></span>|
|<span data-ttu-id="55290-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="55290-154">lastUpdateDateTime</span></span>|<span data-ttu-id="55290-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55290-155">DateTimeOffset</span></span>|<span data-ttu-id="55290-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="55290-156">Last update time</span></span>|
|<span data-ttu-id="55290-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="55290-157">configurationVersion</span></span>|<span data-ttu-id="55290-158">Int32</span><span class="sxs-lookup"><span data-stu-id="55290-158">Int32</span></span>|<span data-ttu-id="55290-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="55290-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="55290-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="55290-160">Response</span></span>
<span data-ttu-id="55290-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55290-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55290-162">Пример</span><span class="sxs-lookup"><span data-stu-id="55290-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="55290-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="55290-163">Request</span></span>
<span data-ttu-id="55290-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55290-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="55290-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="55290-165">Response</span></span>
<span data-ttu-id="55290-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55290-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



