---
title: Создание Виндовсоффицеклиентсекуритиконфигуратион
description: Создание нового объекта Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ac8658489fd27e48866f0d0fa72e222029caf59
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760216"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="92371-103">Создание Виндовсоффицеклиентсекуритиконфигуратион</span><span class="sxs-lookup"><span data-stu-id="92371-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="92371-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92371-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92371-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92371-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92371-106">Создание нового объекта [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="92371-106">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92371-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92371-107">Prerequisites</span></span>
<span data-ttu-id="92371-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92371-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92371-110">Permission type</span></span>|<span data-ttu-id="92371-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92371-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92371-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92371-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92371-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92371-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92371-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92371-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92371-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92371-115">Not supported.</span></span>|
|<span data-ttu-id="92371-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="92371-116">Application</span></span>|<span data-ttu-id="92371-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92371-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92371-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92371-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92371-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92371-119">Request headers</span></span>
|<span data-ttu-id="92371-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92371-120">Header</span></span>|<span data-ttu-id="92371-121">Значение</span><span class="sxs-lookup"><span data-stu-id="92371-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92371-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92371-122">Authorization</span></span>|<span data-ttu-id="92371-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92371-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92371-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92371-124">Accept</span></span>|<span data-ttu-id="92371-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92371-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92371-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92371-126">Request body</span></span>
<span data-ttu-id="92371-127">В тексте запроса добавьте представление объекта [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92371-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="92371-128">В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92371-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="92371-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92371-129">Property</span></span>|<span data-ttu-id="92371-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92371-130">Type</span></span>|<span data-ttu-id="92371-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92371-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92371-132">id</span><span class="sxs-lookup"><span data-stu-id="92371-132">id</span></span>|<span data-ttu-id="92371-133">String</span><span class="sxs-lookup"><span data-stu-id="92371-133">String</span></span>|<span data-ttu-id="92371-134">Идентификатор политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="92371-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="92371-135">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-136">усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="92371-136">userPreferencePayload</span></span>|<span data-ttu-id="92371-137">Stream</span><span class="sxs-lookup"><span data-stu-id="92371-137">Stream</span></span>|<span data-ttu-id="92371-138">Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="92371-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="92371-139">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-140">полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="92371-140">policyPayload</span></span>|<span data-ttu-id="92371-141">Stream</span><span class="sxs-lookup"><span data-stu-id="92371-141">Stream</span></span>|<span data-ttu-id="92371-142">Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="92371-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="92371-143">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-144">description</span><span class="sxs-lookup"><span data-stu-id="92371-144">description</span></span>|<span data-ttu-id="92371-145">String</span><span class="sxs-lookup"><span data-stu-id="92371-145">String</span></span>|<span data-ttu-id="92371-146">Администратор предоставил описание политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="92371-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="92371-147">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-148">displayName</span><span class="sxs-lookup"><span data-stu-id="92371-148">displayName</span></span>|<span data-ttu-id="92371-149">Строка</span><span class="sxs-lookup"><span data-stu-id="92371-149">String</span></span>|<span data-ttu-id="92371-150">Предоставленное администратором имя политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="92371-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="92371-151">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-152">assignments</span><span class="sxs-lookup"><span data-stu-id="92371-152">assignments</span></span>|<span data-ttu-id="92371-153">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92371-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="92371-154">Список назначений групп для политики..</span><span class="sxs-lookup"><span data-stu-id="92371-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="92371-155">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-156">priority</span><span class="sxs-lookup"><span data-stu-id="92371-156">priority</span></span>|<span data-ttu-id="92371-157">Int32</span><span class="sxs-lookup"><span data-stu-id="92371-157">Int32</span></span>|<span data-ttu-id="92371-158">Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="92371-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="92371-159">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92371-160">lastModifiedDateTime</span></span>|<span data-ttu-id="92371-161">DateTime</span><span class="sxs-lookup"><span data-stu-id="92371-161">DateTime</span></span>|<span data-ttu-id="92371-162">Метка даты и времени последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="92371-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="92371-163">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-164">усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="92371-164">userCheckinSummary</span></span>|[<span data-ttu-id="92371-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="92371-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="92371-166">Сводка по возврату пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="92371-166">User check-in summary for the policy.</span></span> <span data-ttu-id="92371-167">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="92371-168">чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="92371-168">checkinStatuses</span></span>|<span data-ttu-id="92371-169">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="92371-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="92371-170">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="92371-170">List of office Client check-in status.</span></span> <span data-ttu-id="92371-171">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92371-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="92371-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="92371-172">Response</span></span>
<span data-ttu-id="92371-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92371-173">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92371-174">Пример</span><span class="sxs-lookup"><span data-stu-id="92371-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="92371-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="92371-175">Request</span></span>
<span data-ttu-id="92371-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92371-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92371-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="92371-177">Response</span></span>
<span data-ttu-id="92371-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92371-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




