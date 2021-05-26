---
title: Создание windowsOfficeClientSecurityConfiguration
description: Создайте новый объект WindowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c4bfcaf3c99c3b587dcf2e6476a848c8098f78f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667070"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="c63b7-103">Создание windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="c63b7-103">Create windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="c63b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c63b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c63b7-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c63b7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c63b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63b7-107">Создайте [новый объект WindowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c63b7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c63b7-108">Prerequisites</span></span>
<span data-ttu-id="c63b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c63b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c63b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c63b7-111">Permission type</span></span>|<span data-ttu-id="c63b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c63b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c63b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c63b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c63b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c63b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c63b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c63b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c63b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63b7-116">Not supported.</span></span>|
|<span data-ttu-id="c63b7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c63b7-117">Application</span></span>|<span data-ttu-id="c63b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c63b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c63b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c63b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c63b7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c63b7-120">Request headers</span></span>
|<span data-ttu-id="c63b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c63b7-121">Header</span></span>|<span data-ttu-id="c63b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c63b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c63b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c63b7-123">Authorization</span></span>|<span data-ttu-id="c63b7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c63b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c63b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c63b7-125">Accept</span></span>|<span data-ttu-id="c63b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c63b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c63b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c63b7-127">Request body</span></span>
<span data-ttu-id="c63b7-128">В теле запроса поставляем представление JSON для [объекта WindowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="c63b7-129">В следующей таблице показаны свойства, необходимые при создании [windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="c63b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c63b7-130">Property</span></span>|<span data-ttu-id="c63b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c63b7-131">Type</span></span>|<span data-ttu-id="c63b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c63b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63b7-133">id</span><span class="sxs-lookup"><span data-stu-id="c63b7-133">id</span></span>|<span data-ttu-id="c63b7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c63b7-134">String</span></span>|<span data-ttu-id="c63b7-135">Id политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="c63b7-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="c63b7-136">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="c63b7-137">userPreferencePayload</span></span>|<span data-ttu-id="c63b7-138">Stream</span><span class="sxs-lookup"><span data-stu-id="c63b7-138">Stream</span></span>|<span data-ttu-id="c63b7-139">Параметры параметров JSON строки в двоичном формате, эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="c63b7-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="c63b7-140">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="c63b7-141">policyPayload</span></span>|<span data-ttu-id="c63b7-142">Stream</span><span class="sxs-lookup"><span data-stu-id="c63b7-142">Stream</span></span>|<span data-ttu-id="c63b7-143">Параметры JSON строки JSON в двоичном формате, эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="c63b7-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="c63b7-144">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-145">description</span><span class="sxs-lookup"><span data-stu-id="c63b7-145">description</span></span>|<span data-ttu-id="c63b7-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c63b7-146">String</span></span>|<span data-ttu-id="c63b7-147">Администратор предоставил описание политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="c63b7-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="c63b7-148">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-149">displayName</span><span class="sxs-lookup"><span data-stu-id="c63b7-149">displayName</span></span>|<span data-ttu-id="c63b7-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c63b7-150">String</span></span>|<span data-ttu-id="c63b7-151">Администратор предоставил имя политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="c63b7-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="c63b7-152">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-153">assignments</span><span class="sxs-lookup"><span data-stu-id="c63b7-153">assignments</span></span>|<span data-ttu-id="c63b7-154">[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c63b7-155">Список групповых назначений для политики..</span><span class="sxs-lookup"><span data-stu-id="c63b7-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="c63b7-156">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-157">priority</span><span class="sxs-lookup"><span data-stu-id="c63b7-157">priority</span></span>|<span data-ttu-id="c63b7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c63b7-158">Int32</span></span>|<span data-ttu-id="c63b7-159">Значение приоритета должно быть уникальным значением для каждой политики клиента и использоваться для разрешения конфликтов, более низкие значения означают высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="c63b7-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="c63b7-160">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c63b7-161">lastModifiedDateTime</span></span>|<span data-ttu-id="c63b7-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="c63b7-162">DateTime</span></span>|<span data-ttu-id="c63b7-163">Последний измененный штамп даты политики.</span><span class="sxs-lookup"><span data-stu-id="c63b7-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="c63b7-164">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c63b7-165">userCheckinSummary</span></span>|[<span data-ttu-id="c63b7-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c63b7-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="c63b7-167">Сводка регистрации пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="c63b7-167">User check-in summary for the policy.</span></span> <span data-ttu-id="c63b7-168">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="c63b7-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="c63b7-169">checkinStatuses</span></span>|<span data-ttu-id="c63b7-170">[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="c63b7-171">Список состояния регистрации клиента office.</span><span class="sxs-lookup"><span data-stu-id="c63b7-171">List of office Client check-in status.</span></span> <span data-ttu-id="c63b7-172">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c63b7-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="c63b7-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="c63b7-173">Response</span></span>
<span data-ttu-id="c63b7-174">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c63b7-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c63b7-175">Пример</span><span class="sxs-lookup"><span data-stu-id="c63b7-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="c63b7-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="c63b7-176">Request</span></span>
<span data-ttu-id="c63b7-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c63b7-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1028

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c63b7-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c63b7-178">Response</span></span>
<span data-ttu-id="c63b7-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c63b7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1077

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
  "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```




