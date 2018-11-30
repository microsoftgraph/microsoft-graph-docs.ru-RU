---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
ms.openlocfilehash: 179f2de37fab17a6ef37a60d00c6b2c566906f9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024704"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="bc834-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="bc834-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="bc834-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc834-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc834-105">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="bc834-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc834-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bc834-106">Prerequisites</span></span>
<span data-ttu-id="bc834-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc834-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc834-109">Permission type</span></span>|<span data-ttu-id="bc834-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc834-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc834-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc834-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc834-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc834-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bc834-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc834-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc834-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc834-114">Not supported.</span></span>|
|<span data-ttu-id="bc834-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc834-115">Application</span></span>|<span data-ttu-id="bc834-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc834-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc834-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc834-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="bc834-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc834-118">Request headers</span></span>
|<span data-ttu-id="bc834-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc834-119">Header</span></span>|<span data-ttu-id="bc834-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bc834-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc834-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc834-121">Authorization</span></span>|<span data-ttu-id="bc834-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bc834-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc834-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bc834-123">Accept</span></span>|<span data-ttu-id="bc834-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc834-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc834-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc834-125">Request body</span></span>
<span data-ttu-id="bc834-126">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc834-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="bc834-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="bc834-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="bc834-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc834-128">Property</span></span>|<span data-ttu-id="bc834-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bc834-129">Type</span></span>|<span data-ttu-id="bc834-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bc834-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc834-131">id</span><span class="sxs-lookup"><span data-stu-id="bc834-131">id</span></span>|<span data-ttu-id="bc834-132">String</span><span class="sxs-lookup"><span data-stu-id="bc834-132">String</span></span>|<span data-ttu-id="bc834-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc834-133">Key of the entity.</span></span>|
|<span data-ttu-id="bc834-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bc834-134">pendingCount</span></span>|<span data-ttu-id="bc834-135">Int32</span><span class="sxs-lookup"><span data-stu-id="bc834-135">Int32</span></span>|<span data-ttu-id="bc834-136">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="bc834-136">Number of pending Users</span></span>|
|<span data-ttu-id="bc834-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bc834-137">notApplicableCount</span></span>|<span data-ttu-id="bc834-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bc834-138">Int32</span></span>|<span data-ttu-id="bc834-139">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="bc834-139">Number of not applicable users</span></span>|
|<span data-ttu-id="bc834-140">successCount</span><span class="sxs-lookup"><span data-stu-id="bc834-140">successCount</span></span>|<span data-ttu-id="bc834-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bc834-141">Int32</span></span>|<span data-ttu-id="bc834-142">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="bc834-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="bc834-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="bc834-143">errorCount</span></span>|<span data-ttu-id="bc834-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bc834-144">Int32</span></span>|<span data-ttu-id="bc834-145">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bc834-145">Number of error Users</span></span>|
|<span data-ttu-id="bc834-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="bc834-146">failedCount</span></span>|<span data-ttu-id="bc834-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bc834-147">Int32</span></span>|<span data-ttu-id="bc834-148">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="bc834-148">Number of failed Users</span></span>|
|<span data-ttu-id="bc834-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bc834-149">lastUpdateDateTime</span></span>|<span data-ttu-id="bc834-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc834-150">DateTimeOffset</span></span>|<span data-ttu-id="bc834-151">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="bc834-151">Last update time</span></span>|
|<span data-ttu-id="bc834-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bc834-152">configurationVersion</span></span>|<span data-ttu-id="bc834-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bc834-153">Int32</span></span>|<span data-ttu-id="bc834-154">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="bc834-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="bc834-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc834-155">Response</span></span>
<span data-ttu-id="bc834-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc834-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc834-157">Пример</span><span class="sxs-lookup"><span data-stu-id="bc834-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc834-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc834-158">Request</span></span>
<span data-ttu-id="bc834-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc834-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="bc834-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc834-160">Response</span></span>
<span data-ttu-id="bc834-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bc834-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



