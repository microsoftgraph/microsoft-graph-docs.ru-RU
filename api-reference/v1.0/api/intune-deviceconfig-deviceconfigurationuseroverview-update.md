---
title: Обновление объекта deviceConfigurationUserOverview
description: Обновление свойств объекта deviceConfigurationUserOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 31dacd98f47062be5e3f20061a6a8f57df985eac
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368584"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="366a9-103">Обновление объекта deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="366a9-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="366a9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="366a9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="366a9-105">Обновление свойств объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="366a9-105">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="366a9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="366a9-106">Prerequisites</span></span>
<span data-ttu-id="366a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="366a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="366a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="366a9-109">Permission type</span></span>|<span data-ttu-id="366a9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="366a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="366a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="366a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="366a9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="366a9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="366a9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="366a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="366a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="366a9-114">Not supported.</span></span>|
|<span data-ttu-id="366a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="366a9-115">Application</span></span>|<span data-ttu-id="366a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="366a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="366a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="366a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="366a9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="366a9-118">Request headers</span></span>
|<span data-ttu-id="366a9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="366a9-119">Header</span></span>|<span data-ttu-id="366a9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="366a9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="366a9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="366a9-121">Authorization</span></span>|<span data-ttu-id="366a9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="366a9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="366a9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="366a9-123">Accept</span></span>|<span data-ttu-id="366a9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="366a9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="366a9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="366a9-125">Request body</span></span>
<span data-ttu-id="366a9-126">В тексте запроса добавьте представление объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="366a9-126">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="366a9-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="366a9-127">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="366a9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="366a9-128">Property</span></span>|<span data-ttu-id="366a9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="366a9-129">Type</span></span>|<span data-ttu-id="366a9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="366a9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="366a9-131">id</span><span class="sxs-lookup"><span data-stu-id="366a9-131">id</span></span>|<span data-ttu-id="366a9-132">String</span><span class="sxs-lookup"><span data-stu-id="366a9-132">String</span></span>|<span data-ttu-id="366a9-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="366a9-133">Key of the entity.</span></span>|
|<span data-ttu-id="366a9-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="366a9-134">pendingCount</span></span>|<span data-ttu-id="366a9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="366a9-135">Int32</span></span>|<span data-ttu-id="366a9-136">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="366a9-136">Number of pending Users</span></span>|
|<span data-ttu-id="366a9-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="366a9-137">notApplicableCount</span></span>|<span data-ttu-id="366a9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="366a9-138">Int32</span></span>|<span data-ttu-id="366a9-139">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="366a9-139">Number of not applicable users</span></span>|
|<span data-ttu-id="366a9-140">successCount</span><span class="sxs-lookup"><span data-stu-id="366a9-140">successCount</span></span>|<span data-ttu-id="366a9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="366a9-141">Int32</span></span>|<span data-ttu-id="366a9-142">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="366a9-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="366a9-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="366a9-143">errorCount</span></span>|<span data-ttu-id="366a9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="366a9-144">Int32</span></span>|<span data-ttu-id="366a9-145">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="366a9-145">Number of error Users</span></span>|
|<span data-ttu-id="366a9-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="366a9-146">failedCount</span></span>|<span data-ttu-id="366a9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="366a9-147">Int32</span></span>|<span data-ttu-id="366a9-148">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="366a9-148">Number of failed Users</span></span>|
|<span data-ttu-id="366a9-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="366a9-149">lastUpdateDateTime</span></span>|<span data-ttu-id="366a9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="366a9-150">DateTimeOffset</span></span>|<span data-ttu-id="366a9-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="366a9-151">Last update time</span></span>|
|<span data-ttu-id="366a9-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="366a9-152">configurationVersion</span></span>|<span data-ttu-id="366a9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="366a9-153">Int32</span></span>|<span data-ttu-id="366a9-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="366a9-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="366a9-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="366a9-155">Response</span></span>
<span data-ttu-id="366a9-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="366a9-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="366a9-157">Пример</span><span class="sxs-lookup"><span data-stu-id="366a9-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="366a9-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="366a9-158">Request</span></span>
<span data-ttu-id="366a9-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="366a9-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="366a9-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="366a9-160">Response</span></span>
<span data-ttu-id="366a9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="366a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




