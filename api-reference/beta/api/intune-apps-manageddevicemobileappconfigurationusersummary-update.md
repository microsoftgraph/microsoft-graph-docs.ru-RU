---
title: Обновление объекта managedDeviceMobileAppConfigurationUserSummary
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b5386c6a385ef499ea92f22ac20cd79a999f833
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397668"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="a578b-103">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="a578b-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="a578b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a578b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a578b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a578b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a578b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a578b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a578b-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="a578b-107">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a578b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a578b-108">Prerequisites</span></span>
<span data-ttu-id="a578b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a578b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a578b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a578b-111">Permission type</span></span>|<span data-ttu-id="a578b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a578b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a578b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a578b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a578b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a578b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a578b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a578b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a578b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a578b-116">Not supported.</span></span>|
|<span data-ttu-id="a578b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a578b-117">Application</span></span>|<span data-ttu-id="a578b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a578b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a578b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a578b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a578b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a578b-120">Request headers</span></span>
|<span data-ttu-id="a578b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a578b-121">Header</span></span>|<span data-ttu-id="a578b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a578b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a578b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a578b-123">Authorization</span></span>|<span data-ttu-id="a578b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a578b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a578b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a578b-125">Accept</span></span>|<span data-ttu-id="a578b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a578b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a578b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a578b-127">Request body</span></span>
<span data-ttu-id="a578b-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a578b-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="a578b-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="a578b-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="a578b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a578b-130">Property</span></span>|<span data-ttu-id="a578b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a578b-131">Type</span></span>|<span data-ttu-id="a578b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a578b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a578b-133">id</span><span class="sxs-lookup"><span data-stu-id="a578b-133">id</span></span>|<span data-ttu-id="a578b-134">String</span><span class="sxs-lookup"><span data-stu-id="a578b-134">String</span></span>|<span data-ttu-id="a578b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a578b-135">Key of the entity.</span></span>|
|<span data-ttu-id="a578b-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="a578b-136">pendingCount</span></span>|<span data-ttu-id="a578b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-137">Int32</span></span>|<span data-ttu-id="a578b-138">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="a578b-138">Number of pending Users</span></span>|
|<span data-ttu-id="a578b-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="a578b-139">notApplicableCount</span></span>|<span data-ttu-id="a578b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-140">Int32</span></span>|<span data-ttu-id="a578b-141">Число пользователей не применим</span><span class="sxs-lookup"><span data-stu-id="a578b-141">Number of not applicable users</span></span>|
|<span data-ttu-id="a578b-142">successCount</span><span class="sxs-lookup"><span data-stu-id="a578b-142">successCount</span></span>|<span data-ttu-id="a578b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-143">Int32</span></span>|<span data-ttu-id="a578b-144">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="a578b-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="a578b-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="a578b-145">errorCount</span></span>|<span data-ttu-id="a578b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-146">Int32</span></span>|<span data-ttu-id="a578b-147">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a578b-147">Number of error Users</span></span>|
|<span data-ttu-id="a578b-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="a578b-148">failedCount</span></span>|<span data-ttu-id="a578b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-149">Int32</span></span>|<span data-ttu-id="a578b-150">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="a578b-150">Number of failed Users</span></span>|
|<span data-ttu-id="a578b-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="a578b-151">conflictCount</span></span>|<span data-ttu-id="a578b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-152">Int32</span></span>|<span data-ttu-id="a578b-153">Количество пользователей в конфликта</span><span class="sxs-lookup"><span data-stu-id="a578b-153">Number of users in conflict</span></span>|
|<span data-ttu-id="a578b-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a578b-154">lastUpdateDateTime</span></span>|<span data-ttu-id="a578b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a578b-155">DateTimeOffset</span></span>|<span data-ttu-id="a578b-156">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="a578b-156">Last update time</span></span>|
|<span data-ttu-id="a578b-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="a578b-157">configurationVersion</span></span>|<span data-ttu-id="a578b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a578b-158">Int32</span></span>|<span data-ttu-id="a578b-159">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="a578b-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="a578b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a578b-160">Response</span></span>
<span data-ttu-id="a578b-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a578b-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a578b-162">Пример</span><span class="sxs-lookup"><span data-stu-id="a578b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a578b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="a578b-163">Request</span></span>
<span data-ttu-id="a578b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a578b-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 321

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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

### <a name="response"></a><span data-ttu-id="a578b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a578b-165">Response</span></span>
<span data-ttu-id="a578b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a578b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
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




