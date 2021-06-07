---
title: Создание windowsOfficeClientConfiguration
description: Создайте новую политику небезопасности с целевыми группами.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 159a99785a63e74f863c977a8c0bfe933f8ced75
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754393"
---
# <a name="create-windowsofficeclientconfiguration"></a><span data-ttu-id="3a1d5-103">Создание windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a1d5-103">Create windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="3a1d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a1d5-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a1d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a1d5-107">Создайте новую политику небезопасности с целевыми группами.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-107">Create a new non-security policy with targeting groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a1d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a1d5-108">Prerequisites</span></span>
<span data-ttu-id="3a1d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a1d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a1d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a1d5-111">Permission type</span></span>|<span data-ttu-id="3a1d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a1d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a1d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a1d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a1d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a1d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-116">Not supported.</span></span>|
|<span data-ttu-id="3a1d5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a1d5-117">Application</span></span>|<span data-ttu-id="3a1d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a1d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a1d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a1d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3a1d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a1d5-120">Request headers</span></span>
|<span data-ttu-id="3a1d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a1d5-121">Header</span></span>|<span data-ttu-id="3a1d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a1d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a1d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a1d5-123">Authorization</span></span>|<span data-ttu-id="3a1d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a1d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a1d5-125">Accept</span></span>|<span data-ttu-id="3a1d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a1d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a1d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a1d5-127">Request body</span></span>
<span data-ttu-id="3a1d5-128">В теле запроса предоставляем представление JSON для [объекта WindowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="3a1d5-129">В следующей таблице показаны свойства, необходимые при создании [windowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="3a1d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a1d5-130">Property</span></span>|<span data-ttu-id="3a1d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a1d5-131">Type</span></span>|<span data-ttu-id="3a1d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a1d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a1d5-133">id</span><span class="sxs-lookup"><span data-stu-id="3a1d5-133">id</span></span>|<span data-ttu-id="3a1d5-134">String</span><span class="sxs-lookup"><span data-stu-id="3a1d5-134">String</span></span>|<span data-ttu-id="3a1d5-135">Id политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="3a1d5-136">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-137">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="3a1d5-137">userPreferencePayload</span></span>|<span data-ttu-id="3a1d5-138">Stream</span><span class="sxs-lookup"><span data-stu-id="3a1d5-138">Stream</span></span>|<span data-ttu-id="3a1d5-139">Параметры параметров JSON строки в двоичном формате, эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="3a1d5-140">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-141">policyPayload</span><span class="sxs-lookup"><span data-stu-id="3a1d5-141">policyPayload</span></span>|<span data-ttu-id="3a1d5-142">Stream</span><span class="sxs-lookup"><span data-stu-id="3a1d5-142">Stream</span></span>|<span data-ttu-id="3a1d5-143">Параметры JSON строки JSON в двоичном формате, эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="3a1d5-144">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-145">description</span><span class="sxs-lookup"><span data-stu-id="3a1d5-145">description</span></span>|<span data-ttu-id="3a1d5-146">String</span><span class="sxs-lookup"><span data-stu-id="3a1d5-146">String</span></span>|<span data-ttu-id="3a1d5-147">Администратор предоставил описание политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="3a1d5-148">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-149">displayName</span><span class="sxs-lookup"><span data-stu-id="3a1d5-149">displayName</span></span>|<span data-ttu-id="3a1d5-150">String</span><span class="sxs-lookup"><span data-stu-id="3a1d5-150">String</span></span>|<span data-ttu-id="3a1d5-151">Администратор предоставил имя политики конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="3a1d5-152">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-153">assignments</span><span class="sxs-lookup"><span data-stu-id="3a1d5-153">assignments</span></span>|<span data-ttu-id="3a1d5-154">[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3a1d5-155">Список групповых назначений для политики..</span><span class="sxs-lookup"><span data-stu-id="3a1d5-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="3a1d5-156">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-157">priority</span><span class="sxs-lookup"><span data-stu-id="3a1d5-157">priority</span></span>|<span data-ttu-id="3a1d5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3a1d5-158">Int32</span></span>|<span data-ttu-id="3a1d5-159">Значение приоритета должно быть уникальным значением для каждой политики клиента и использоваться для разрешения конфликтов, более низкие значения означают высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="3a1d5-160">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a1d5-161">lastModifiedDateTime</span></span>|<span data-ttu-id="3a1d5-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="3a1d5-162">DateTime</span></span>|<span data-ttu-id="3a1d5-163">Последний измененный штамп даты политики.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="3a1d5-164">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-165">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3a1d5-165">userCheckinSummary</span></span>|[<span data-ttu-id="3a1d5-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3a1d5-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="3a1d5-167">Сводка регистрации пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-167">User check-in summary for the policy.</span></span> <span data-ttu-id="3a1d5-168">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3a1d5-169">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="3a1d5-169">checkinStatuses</span></span>|<span data-ttu-id="3a1d5-170">[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="3a1d5-171">Список состояния регистрации клиента office.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-171">List of office Client check-in status.</span></span> <span data-ttu-id="3a1d5-172">Унаследованный от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a1d5-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3a1d5-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1d5-173">Response</span></span>
<span data-ttu-id="3a1d5-174">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a1d5-175">Пример</span><span class="sxs-lookup"><span data-stu-id="3a1d5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a1d5-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a1d5-176">Request</span></span>
<span data-ttu-id="3a1d5-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
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

### <a name="response"></a><span data-ttu-id="3a1d5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1d5-178">Response</span></span>
<span data-ttu-id="3a1d5-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a1d5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
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




