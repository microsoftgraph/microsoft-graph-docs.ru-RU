---
title: Обновление Виндовсоффицеклиентконфигуратион
description: Обновление определенных полезных данных политики, не связанных с безопасностью.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09c663609e80ac3db7e85fe3f2e35cac33745bd7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322165"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="0cd19-103">Обновление Виндовсоффицеклиентконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0cd19-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="0cd19-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cd19-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cd19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd19-106">Обновление определенных полезных данных политики, не связанных с безопасностью.</span><span class="sxs-lookup"><span data-stu-id="0cd19-106">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd19-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0cd19-107">Prerequisites</span></span>
<span data-ttu-id="0cd19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd19-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd19-110">Permission type</span></span>|<span data-ttu-id="0cd19-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cd19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd19-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cd19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd19-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd19-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cd19-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cd19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd19-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd19-115">Not supported.</span></span>|
|<span data-ttu-id="0cd19-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cd19-116">Application</span></span>|<span data-ttu-id="0cd19-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd19-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd19-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cd19-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="0cd19-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cd19-119">Request headers</span></span>
|<span data-ttu-id="0cd19-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cd19-120">Header</span></span>|<span data-ttu-id="0cd19-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0cd19-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd19-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cd19-122">Authorization</span></span>|<span data-ttu-id="0cd19-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cd19-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd19-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0cd19-124">Accept</span></span>|<span data-ttu-id="0cd19-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd19-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd19-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0cd19-126">Request body</span></span>
<span data-ttu-id="0cd19-127">В тексте запроса добавьте представление объекта [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cd19-127">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="0cd19-128">В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0cd19-128">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="0cd19-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd19-129">Property</span></span>|<span data-ttu-id="0cd19-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0cd19-130">Type</span></span>|<span data-ttu-id="0cd19-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd19-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cd19-132">id</span><span class="sxs-lookup"><span data-stu-id="0cd19-132">id</span></span>|<span data-ttu-id="0cd19-133">String</span><span class="sxs-lookup"><span data-stu-id="0cd19-133">String</span></span>|<span data-ttu-id="0cd19-134">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-134">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-135">усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="0cd19-135">userPreferencePayload</span></span>|<span data-ttu-id="0cd19-136">Поток</span><span class="sxs-lookup"><span data-stu-id="0cd19-136">Stream</span></span>|<span data-ttu-id="0cd19-137">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-137">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-138">полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="0cd19-138">policyPayload</span></span>|<span data-ttu-id="0cd19-139">Поток</span><span class="sxs-lookup"><span data-stu-id="0cd19-139">Stream</span></span>|<span data-ttu-id="0cd19-140">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-140">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-141">description</span><span class="sxs-lookup"><span data-stu-id="0cd19-141">description</span></span>|<span data-ttu-id="0cd19-142">String</span><span class="sxs-lookup"><span data-stu-id="0cd19-142">String</span></span>|<span data-ttu-id="0cd19-143">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-143">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0cd19-144">displayName</span></span>|<span data-ttu-id="0cd19-145">Строка</span><span class="sxs-lookup"><span data-stu-id="0cd19-145">String</span></span>|<span data-ttu-id="0cd19-146">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-146">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-147">priority</span><span class="sxs-lookup"><span data-stu-id="0cd19-147">priority</span></span>|<span data-ttu-id="0cd19-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0cd19-148">Int32</span></span>|<span data-ttu-id="0cd19-149">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-149">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-150">усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="0cd19-150">userCheckinSummary</span></span>|[<span data-ttu-id="0cd19-151">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="0cd19-151">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="0cd19-152">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-152">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="0cd19-153">чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="0cd19-153">checkinStatuses</span></span>|<span data-ttu-id="0cd19-154">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-154">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="0cd19-155">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cd19-155">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0cd19-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd19-156">Response</span></span>
<span data-ttu-id="0cd19-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cd19-157">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd19-158">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd19-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd19-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cd19-159">Request</span></span>
<span data-ttu-id="0cd19-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cd19-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}
Content-type: application/json
Content-length: 949

{
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

### <a name="response"></a><span data-ttu-id="0cd19-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd19-161">Response</span></span>
<span data-ttu-id="0cd19-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






