---
title: Создание Виндовсоффицеклиентсекуритиконфигуратион
description: Создание нового объекта Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a9726794d88dfb742077b9a5b94fc226265b1b4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170695"
---
# <a name="create-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="7d951-103">Создание Виндовсоффицеклиентсекуритиконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7d951-103">Create windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="7d951-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d951-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d951-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d951-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d951-106">Создание нового объекта [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7d951-106">Create a new [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d951-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d951-107">Prerequisites</span></span>
<span data-ttu-id="7d951-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d951-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d951-110">Permission type</span></span>|<span data-ttu-id="7d951-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d951-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d951-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d951-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d951-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d951-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d951-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d951-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d951-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d951-115">Not supported.</span></span>|
|<span data-ttu-id="7d951-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d951-116">Application</span></span>|<span data-ttu-id="7d951-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d951-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d951-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d951-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7d951-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d951-119">Request headers</span></span>
|<span data-ttu-id="7d951-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d951-120">Header</span></span>|<span data-ttu-id="7d951-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7d951-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d951-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d951-122">Authorization</span></span>|<span data-ttu-id="7d951-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d951-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d951-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7d951-124">Accept</span></span>|<span data-ttu-id="7d951-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d951-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d951-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d951-126">Request body</span></span>
<span data-ttu-id="7d951-127">В тексте запроса добавьте представление объекта [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d951-127">In the request body, supply a JSON representation for the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

<span data-ttu-id="7d951-128">В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d951-128">The following table shows the properties that are required when you create the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

|<span data-ttu-id="7d951-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d951-129">Property</span></span>|<span data-ttu-id="7d951-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7d951-130">Type</span></span>|<span data-ttu-id="7d951-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7d951-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d951-132">id</span><span class="sxs-lookup"><span data-stu-id="7d951-132">id</span></span>|<span data-ttu-id="7d951-133">String</span><span class="sxs-lookup"><span data-stu-id="7d951-133">String</span></span>|<span data-ttu-id="7d951-134">Идентификатор политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="7d951-134">Id of the office client configuration policy.</span></span> <span data-ttu-id="7d951-135">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-135">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-136">усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="7d951-136">userPreferencePayload</span></span>|<span data-ttu-id="7d951-137">Поток</span><span class="sxs-lookup"><span data-stu-id="7d951-137">Stream</span></span>|<span data-ttu-id="7d951-138">Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем.</span><span class="sxs-lookup"><span data-stu-id="7d951-138">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span> <span data-ttu-id="7d951-139">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-139">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-140">полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="7d951-140">policyPayload</span></span>|<span data-ttu-id="7d951-141">Поток</span><span class="sxs-lookup"><span data-stu-id="7d951-141">Stream</span></span>|<span data-ttu-id="7d951-142">Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем.</span><span class="sxs-lookup"><span data-stu-id="7d951-142">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span> <span data-ttu-id="7d951-143">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-143">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-144">description</span><span class="sxs-lookup"><span data-stu-id="7d951-144">description</span></span>|<span data-ttu-id="7d951-145">String</span><span class="sxs-lookup"><span data-stu-id="7d951-145">String</span></span>|<span data-ttu-id="7d951-146">Администратор предоставил описание политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="7d951-146">Admin provided description of the office client configuration policy.</span></span> <span data-ttu-id="7d951-147">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-147">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-148">displayName</span><span class="sxs-lookup"><span data-stu-id="7d951-148">displayName</span></span>|<span data-ttu-id="7d951-149">Строка</span><span class="sxs-lookup"><span data-stu-id="7d951-149">String</span></span>|<span data-ttu-id="7d951-150">Предоставленное администратором имя политики конфигурации клиента Office.</span><span class="sxs-lookup"><span data-stu-id="7d951-150">Admin provided name of the office client configuration policy.</span></span> <span data-ttu-id="7d951-151">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-151">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-152">assignments</span><span class="sxs-lookup"><span data-stu-id="7d951-152">assignments</span></span>|<span data-ttu-id="7d951-153">Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-153">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7d951-154">Список назначений групп для политики..</span><span class="sxs-lookup"><span data-stu-id="7d951-154">The list of group assignments for the policy..</span></span> <span data-ttu-id="7d951-155">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-155">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-156">priority</span><span class="sxs-lookup"><span data-stu-id="7d951-156">priority</span></span>|<span data-ttu-id="7d951-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7d951-157">Int32</span></span>|<span data-ttu-id="7d951-158">Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="7d951-158">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span> <span data-ttu-id="7d951-159">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-159">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d951-160">lastModifiedDateTime</span></span>|<span data-ttu-id="7d951-161">DateTime.</span><span class="sxs-lookup"><span data-stu-id="7d951-161">DateTime</span></span>|<span data-ttu-id="7d951-162">Метка даты и времени последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="7d951-162">Last modified datetime stamp of the policy.</span></span> <span data-ttu-id="7d951-163">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-163">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-164">усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="7d951-164">userCheckinSummary</span></span>|[<span data-ttu-id="7d951-165">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="7d951-165">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="7d951-166">Сводка по возврату пользователя для политики.</span><span class="sxs-lookup"><span data-stu-id="7d951-166">User check-in summary for the policy.</span></span> <span data-ttu-id="7d951-167">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-167">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="7d951-168">чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="7d951-168">checkinStatuses</span></span>|<span data-ttu-id="7d951-169">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-169">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="7d951-170">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="7d951-170">List of office Client check-in status.</span></span> <span data-ttu-id="7d951-171">Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d951-171">Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|




## <a name="response"></a><span data-ttu-id="7d951-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d951-172">Response</span></span>
<span data-ttu-id="7d951-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d951-173">If successful, this method returns a `201 Created` response code and a [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d951-174">Пример</span><span class="sxs-lookup"><span data-stu-id="7d951-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d951-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d951-175">Request</span></span>
<span data-ttu-id="7d951-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d951-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d951-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d951-177">Response</span></span>
<span data-ttu-id="7d951-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d951-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




