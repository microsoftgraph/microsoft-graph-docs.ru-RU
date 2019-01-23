---
title: Обновление объекта deviceConfigurationUserOverview
description: Обновление свойств объекта deviceConfigurationUserOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cedb9b1116024821d22dec7d159cadc602fba08e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412991"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="81153-103">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="81153-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="81153-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81153-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81153-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81153-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81153-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81153-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81153-107">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="81153-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81153-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="81153-108">Prerequisites</span></span>
<span data-ttu-id="81153-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="81153-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="81153-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81153-111">Permission type</span></span>|<span data-ttu-id="81153-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81153-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81153-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81153-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81153-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81153-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81153-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81153-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81153-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81153-116">Not supported.</span></span>|
|<span data-ttu-id="81153-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81153-117">Application</span></span>|<span data-ttu-id="81153-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81153-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81153-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81153-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="81153-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81153-120">Request headers</span></span>
|<span data-ttu-id="81153-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81153-121">Header</span></span>|<span data-ttu-id="81153-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81153-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81153-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81153-123">Authorization</span></span>|<span data-ttu-id="81153-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="81153-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81153-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81153-125">Accept</span></span>|<span data-ttu-id="81153-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81153-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81153-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81153-127">Request body</span></span>
<span data-ttu-id="81153-128">В тексте запроса добавьте представление объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81153-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="81153-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="81153-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="81153-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="81153-130">Property</span></span>|<span data-ttu-id="81153-131">Тип</span><span class="sxs-lookup"><span data-stu-id="81153-131">Type</span></span>|<span data-ttu-id="81153-132">Описание</span><span class="sxs-lookup"><span data-stu-id="81153-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81153-133">id</span><span class="sxs-lookup"><span data-stu-id="81153-133">id</span></span>|<span data-ttu-id="81153-134">String</span><span class="sxs-lookup"><span data-stu-id="81153-134">String</span></span>|<span data-ttu-id="81153-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81153-135">Key of the entity.</span></span>|
|<span data-ttu-id="81153-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="81153-136">pendingCount</span></span>|<span data-ttu-id="81153-137">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-137">Int32</span></span>|<span data-ttu-id="81153-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="81153-138">Number of pending Users</span></span>|
|<span data-ttu-id="81153-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="81153-139">notApplicableCount</span></span>|<span data-ttu-id="81153-140">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-140">Int32</span></span>|<span data-ttu-id="81153-141">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="81153-141">Number of not applicable users</span></span>|
|<span data-ttu-id="81153-142">successCount</span><span class="sxs-lookup"><span data-stu-id="81153-142">successCount</span></span>|<span data-ttu-id="81153-143">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-143">Int32</span></span>|<span data-ttu-id="81153-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="81153-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="81153-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="81153-145">errorCount</span></span>|<span data-ttu-id="81153-146">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-146">Int32</span></span>|<span data-ttu-id="81153-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="81153-147">Number of error Users</span></span>|
|<span data-ttu-id="81153-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="81153-148">failedCount</span></span>|<span data-ttu-id="81153-149">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-149">Int32</span></span>|<span data-ttu-id="81153-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="81153-150">Number of failed Users</span></span>|
|<span data-ttu-id="81153-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="81153-151">conflictCount</span></span>|<span data-ttu-id="81153-152">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-152">Int32</span></span>|<span data-ttu-id="81153-153">Количество пользователей в конфликта</span><span class="sxs-lookup"><span data-stu-id="81153-153">Number of users in conflict</span></span>|
|<span data-ttu-id="81153-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="81153-154">lastUpdateDateTime</span></span>|<span data-ttu-id="81153-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81153-155">DateTimeOffset</span></span>|<span data-ttu-id="81153-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="81153-156">Last update time</span></span>|
|<span data-ttu-id="81153-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="81153-157">configurationVersion</span></span>|<span data-ttu-id="81153-158">Int32</span><span class="sxs-lookup"><span data-stu-id="81153-158">Int32</span></span>|<span data-ttu-id="81153-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="81153-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="81153-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="81153-160">Response</span></span>
<span data-ttu-id="81153-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81153-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81153-162">Пример</span><span class="sxs-lookup"><span data-stu-id="81153-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="81153-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="81153-163">Request</span></span>
<span data-ttu-id="81153-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81153-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="81153-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="81153-165">Response</span></span>
<span data-ttu-id="81153-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="81153-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




