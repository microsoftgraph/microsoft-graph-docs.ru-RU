---
title: Создание Виндовсоффицеклиентсекуритиконфигуратион
description: Создание нового объекта Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f73f14ddf05458faa6ab5a6aa72ea63537547f6a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450253"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="bcc59-103">Создание Виндовсоффицеклиентсекуритиконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bcc59-103">Create windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="bcc59-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcc59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcc59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcc59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcc59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc59-107">Создание нового объекта [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bcc59-107">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcc59-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcc59-108">Prerequisites</span></span>
<span data-ttu-id="bcc59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc59-111">Permission type</span></span>|<span data-ttu-id="bcc59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcc59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcc59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcc59-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcc59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc59-116">Not supported.</span></span>|
|<span data-ttu-id="bcc59-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcc59-117">Application</span></span>|<span data-ttu-id="bcc59-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc59-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcc59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bcc59-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bcc59-120">Request headers</span></span>
|<span data-ttu-id="bcc59-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcc59-121">Header</span></span>|<span data-ttu-id="bcc59-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bcc59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcc59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcc59-123">Authorization</span></span>|<span data-ttu-id="bcc59-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcc59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcc59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bcc59-125">Accept</span></span>|<span data-ttu-id="bcc59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcc59-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcc59-127">Request body</span></span>
<span data-ttu-id="bcc59-128">В тексте запроса добавьте представление объекта [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcc59-128">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="bcc59-129">В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcc59-129">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="bcc59-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcc59-130">Property</span></span>|<span data-ttu-id="bcc59-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc59-131">Type</span></span>|<span data-ttu-id="bcc59-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc59-133">id</span><span class="sxs-lookup"><span data-stu-id="bcc59-133">id</span></span>|<span data-ttu-id="bcc59-134">String</span><span class="sxs-lookup"><span data-stu-id="bcc59-134">String</span></span>|<span data-ttu-id="bcc59-135">Идентификатор политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="bcc59-135">Id of the office client configuration policy.</span></span> <span data-ttu-id="bcc59-136">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-136">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-137">усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="bcc59-137">userPreferencePayload</span></span>|<span data-ttu-id="bcc59-138">Stream</span><span class="sxs-lookup"><span data-stu-id="bcc59-138">Stream</span></span>|<span data-ttu-id="bcc59-139">Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="bcc59-139">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="bcc59-140">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-140">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-141">полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="bcc59-141">policyPayload</span></span>|<span data-ttu-id="bcc59-142">Stream</span><span class="sxs-lookup"><span data-stu-id="bcc59-142">Stream</span></span>|<span data-ttu-id="bcc59-143">Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="bcc59-143">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="bcc59-144">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-144">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-145">description</span><span class="sxs-lookup"><span data-stu-id="bcc59-145">description</span></span>|<span data-ttu-id="bcc59-146">String</span><span class="sxs-lookup"><span data-stu-id="bcc59-146">String</span></span>|<span data-ttu-id="bcc59-147">Администратор предоставил описание политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="bcc59-147">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="bcc59-148">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-148">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-149">displayName</span><span class="sxs-lookup"><span data-stu-id="bcc59-149">displayName</span></span>|<span data-ttu-id="bcc59-150">Строка</span><span class="sxs-lookup"><span data-stu-id="bcc59-150">String</span></span>|<span data-ttu-id="bcc59-151">Предоставленное администратором имя политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="bcc59-151">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="bcc59-152">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-152">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-153">assignments</span><span class="sxs-lookup"><span data-stu-id="bcc59-153">assignments</span></span>|<span data-ttu-id="bcc59-154">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-154">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bcc59-155">Список назначений групп для политики..</span><span class="sxs-lookup"><span data-stu-id="bcc59-155">The list of group assignments for the policy..</span></span> <span data-ttu-id="bcc59-156">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-156">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-157">priority</span><span class="sxs-lookup"><span data-stu-id="bcc59-157">priority</span></span>|<span data-ttu-id="bcc59-158">Int32</span><span class="sxs-lookup"><span data-stu-id="bcc59-158">Int32</span></span>|<span data-ttu-id="bcc59-159">Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="bcc59-159">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="bcc59-160">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-160">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcc59-161">lastModifiedDateTime</span></span>|<span data-ttu-id="bcc59-162">DateTime</span><span class="sxs-lookup"><span data-stu-id="bcc59-162">DateTime</span></span>|<span data-ttu-id="bcc59-163">Метка даты и времени последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bcc59-163">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="bcc59-164">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-164">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-165">усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="bcc59-165">userCheckinSummary</span></span>|[<span data-ttu-id="bcc59-166">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bcc59-166">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="bcc59-167">Сводка по возврату пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="bcc59-167">User check-in summary for the policy.</span></span> <span data-ttu-id="bcc59-168">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-168">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="bcc59-169">чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="bcc59-169">checkinStatuses</span></span>|<span data-ttu-id="bcc59-170">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-170">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="bcc59-171">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="bcc59-171">List of office Client check-in status.</span></span> <span data-ttu-id="bcc59-172">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcc59-172">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="bcc59-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc59-173">Response</span></span>
<span data-ttu-id="bcc59-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc59-174">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc59-175">Пример</span><span class="sxs-lookup"><span data-stu-id="bcc59-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcc59-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc59-176">Request</span></span>
<span data-ttu-id="bcc59-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc59-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcc59-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc59-178">Response</span></span>
<span data-ttu-id="bcc59-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcc59-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





