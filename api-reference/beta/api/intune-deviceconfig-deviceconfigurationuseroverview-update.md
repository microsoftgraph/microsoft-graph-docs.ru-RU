---
title: Обновление объекта deviceConfigurationUserOverview
description: Обновление свойств объекта deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0837767a7855aec4fe60bf9c3d0adfed52b4b368
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156247"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="4e9de-103">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4e9de-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="4e9de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e9de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e9de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e9de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e9de-106">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4e9de-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e9de-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e9de-107">Prerequisites</span></span>
<span data-ttu-id="4e9de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e9de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e9de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e9de-110">Permission type</span></span>|<span data-ttu-id="4e9de-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e9de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e9de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e9de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e9de-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e9de-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e9de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e9de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e9de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e9de-115">Not supported.</span></span>|
|<span data-ttu-id="4e9de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e9de-116">Application</span></span>|<span data-ttu-id="4e9de-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e9de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e9de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e9de-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="4e9de-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e9de-119">Request headers</span></span>
|<span data-ttu-id="4e9de-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e9de-120">Header</span></span>|<span data-ttu-id="4e9de-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e9de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e9de-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e9de-122">Authorization</span></span>|<span data-ttu-id="4e9de-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e9de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e9de-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e9de-124">Accept</span></span>|<span data-ttu-id="4e9de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e9de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e9de-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e9de-126">Request body</span></span>
<span data-ttu-id="4e9de-127">В тексте запроса добавьте представление объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e9de-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="4e9de-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4e9de-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="4e9de-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e9de-129">Property</span></span>|<span data-ttu-id="4e9de-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4e9de-130">Type</span></span>|<span data-ttu-id="4e9de-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e9de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e9de-132">id</span><span class="sxs-lookup"><span data-stu-id="4e9de-132">id</span></span>|<span data-ttu-id="4e9de-133">String</span><span class="sxs-lookup"><span data-stu-id="4e9de-133">String</span></span>|<span data-ttu-id="4e9de-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e9de-134">Key of the entity.</span></span>|
|<span data-ttu-id="4e9de-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4e9de-135">pendingCount</span></span>|<span data-ttu-id="4e9de-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-136">Int32</span></span>|<span data-ttu-id="4e9de-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="4e9de-137">Number of pending Users</span></span>|
|<span data-ttu-id="4e9de-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4e9de-138">notApplicableCount</span></span>|<span data-ttu-id="4e9de-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-139">Int32</span></span>|<span data-ttu-id="4e9de-140">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="4e9de-140">Number of not applicable users</span></span>|
|<span data-ttu-id="4e9de-141">successCount</span><span class="sxs-lookup"><span data-stu-id="4e9de-141">successCount</span></span>|<span data-ttu-id="4e9de-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-142">Int32</span></span>|<span data-ttu-id="4e9de-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4e9de-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="4e9de-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="4e9de-144">errorCount</span></span>|<span data-ttu-id="4e9de-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-145">Int32</span></span>|<span data-ttu-id="4e9de-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4e9de-146">Number of error Users</span></span>|
|<span data-ttu-id="4e9de-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="4e9de-147">failedCount</span></span>|<span data-ttu-id="4e9de-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-148">Int32</span></span>|<span data-ttu-id="4e9de-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="4e9de-149">Number of failed Users</span></span>|
|<span data-ttu-id="4e9de-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4e9de-150">conflictCount</span></span>|<span data-ttu-id="4e9de-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-151">Int32</span></span>|<span data-ttu-id="4e9de-152">Количество пользователей в конфликте</span><span class="sxs-lookup"><span data-stu-id="4e9de-152">Number of users in conflict</span></span>|
|<span data-ttu-id="4e9de-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4e9de-153">lastUpdateDateTime</span></span>|<span data-ttu-id="4e9de-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e9de-154">DateTimeOffset</span></span>|<span data-ttu-id="4e9de-155">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="4e9de-155">Last update time</span></span>|
|<span data-ttu-id="4e9de-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4e9de-156">configurationVersion</span></span>|<span data-ttu-id="4e9de-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4e9de-157">Int32</span></span>|<span data-ttu-id="4e9de-158">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="4e9de-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4e9de-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e9de-159">Response</span></span>
<span data-ttu-id="4e9de-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e9de-160">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e9de-161">Пример</span><span class="sxs-lookup"><span data-stu-id="4e9de-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e9de-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e9de-162">Request</span></span>
<span data-ttu-id="4e9de-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e9de-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e9de-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e9de-164">Response</span></span>
<span data-ttu-id="4e9de-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e9de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




