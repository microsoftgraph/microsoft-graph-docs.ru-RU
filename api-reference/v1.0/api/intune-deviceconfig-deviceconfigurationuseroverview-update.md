---
title: Обновление объекта deviceConfigurationUserOverview
description: Обновление свойств объекта deviceConfigurationUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b91c8ff52a39c6810a833042f7ed5d6e78a910d6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760624"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="727c1-103">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="727c1-103">Update deviceConfigurationUserOverview</span></span>

<span data-ttu-id="727c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="727c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="727c1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="727c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="727c1-106">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="727c1-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="727c1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="727c1-107">Prerequisites</span></span>
<span data-ttu-id="727c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="727c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="727c1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="727c1-110">Permission type</span></span>|<span data-ttu-id="727c1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="727c1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="727c1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="727c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="727c1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="727c1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="727c1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="727c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="727c1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="727c1-115">Not supported.</span></span>|
|<span data-ttu-id="727c1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="727c1-116">Application</span></span>|<span data-ttu-id="727c1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="727c1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="727c1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="727c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="727c1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="727c1-119">Request headers</span></span>
|<span data-ttu-id="727c1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="727c1-120">Header</span></span>|<span data-ttu-id="727c1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="727c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="727c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="727c1-122">Authorization</span></span>|<span data-ttu-id="727c1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="727c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="727c1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="727c1-124">Accept</span></span>|<span data-ttu-id="727c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="727c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="727c1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="727c1-126">Request body</span></span>
<span data-ttu-id="727c1-127">В тексте запроса добавьте представление объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="727c1-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="727c1-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="727c1-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="727c1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="727c1-129">Property</span></span>|<span data-ttu-id="727c1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="727c1-130">Type</span></span>|<span data-ttu-id="727c1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="727c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="727c1-132">id</span><span class="sxs-lookup"><span data-stu-id="727c1-132">id</span></span>|<span data-ttu-id="727c1-133">String</span><span class="sxs-lookup"><span data-stu-id="727c1-133">String</span></span>|<span data-ttu-id="727c1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="727c1-134">Key of the entity.</span></span>|
|<span data-ttu-id="727c1-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="727c1-135">pendingCount</span></span>|<span data-ttu-id="727c1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="727c1-136">Int32</span></span>|<span data-ttu-id="727c1-137">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="727c1-137">Number of pending Users</span></span>|
|<span data-ttu-id="727c1-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="727c1-138">notApplicableCount</span></span>|<span data-ttu-id="727c1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="727c1-139">Int32</span></span>|<span data-ttu-id="727c1-140">Число не применимых пользователей</span><span class="sxs-lookup"><span data-stu-id="727c1-140">Number of not applicable users</span></span>|
|<span data-ttu-id="727c1-141">successCount</span><span class="sxs-lookup"><span data-stu-id="727c1-141">successCount</span></span>|<span data-ttu-id="727c1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="727c1-142">Int32</span></span>|<span data-ttu-id="727c1-143">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="727c1-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="727c1-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="727c1-144">errorCount</span></span>|<span data-ttu-id="727c1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="727c1-145">Int32</span></span>|<span data-ttu-id="727c1-146">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="727c1-146">Number of error Users</span></span>|
|<span data-ttu-id="727c1-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="727c1-147">failedCount</span></span>|<span data-ttu-id="727c1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="727c1-148">Int32</span></span>|<span data-ttu-id="727c1-149">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="727c1-149">Number of failed Users</span></span>|
|<span data-ttu-id="727c1-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="727c1-150">lastUpdateDateTime</span></span>|<span data-ttu-id="727c1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="727c1-151">DateTimeOffset</span></span>|<span data-ttu-id="727c1-152">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="727c1-152">Last update time</span></span>|
|<span data-ttu-id="727c1-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="727c1-153">configurationVersion</span></span>|<span data-ttu-id="727c1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="727c1-154">Int32</span></span>|<span data-ttu-id="727c1-155">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="727c1-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="727c1-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="727c1-156">Response</span></span>
<span data-ttu-id="727c1-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="727c1-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="727c1-158">Пример</span><span class="sxs-lookup"><span data-stu-id="727c1-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="727c1-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="727c1-159">Request</span></span>
<span data-ttu-id="727c1-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="727c1-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 282

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="727c1-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="727c1-161">Response</span></span>
<span data-ttu-id="727c1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="727c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




