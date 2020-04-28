---
title: Обновление Виндовсоффицеклиентконфигуратион
description: Обновление определенных полезных данных политики, не связанных с безопасностью.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81d75e24cd6e6687b081ed77a7195ab6bad08c2d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436693"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="16730-103">Обновление Виндовсоффицеклиентконфигуратион</span><span class="sxs-lookup"><span data-stu-id="16730-103">Update windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="16730-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16730-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16730-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16730-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16730-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16730-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16730-107">Обновление определенных полезных данных политики, не связанных с безопасностью.</span><span class="sxs-lookup"><span data-stu-id="16730-107">Patch a specific non-security policy payload.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16730-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16730-108">Prerequisites</span></span>
<span data-ttu-id="16730-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16730-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16730-111">Permission type</span></span>|<span data-ttu-id="16730-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16730-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16730-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16730-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16730-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16730-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16730-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16730-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16730-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16730-116">Not supported.</span></span>|
|<span data-ttu-id="16730-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16730-117">Application</span></span>|<span data-ttu-id="16730-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16730-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16730-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16730-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="16730-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16730-120">Request headers</span></span>
|<span data-ttu-id="16730-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16730-121">Header</span></span>|<span data-ttu-id="16730-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16730-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16730-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16730-123">Authorization</span></span>|<span data-ttu-id="16730-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16730-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16730-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16730-125">Accept</span></span>|<span data-ttu-id="16730-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16730-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16730-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16730-127">Request body</span></span>
<span data-ttu-id="16730-128">В тексте запроса добавьте представление объекта [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16730-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="16730-129">В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="16730-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="16730-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16730-130">Property</span></span>|<span data-ttu-id="16730-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16730-131">Type</span></span>|<span data-ttu-id="16730-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16730-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16730-133">id</span><span class="sxs-lookup"><span data-stu-id="16730-133">id</span></span>|<span data-ttu-id="16730-134">String</span><span class="sxs-lookup"><span data-stu-id="16730-134">String</span></span>|<span data-ttu-id="16730-135">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-136">усерпреференцепайлоад</span><span class="sxs-lookup"><span data-stu-id="16730-136">userPreferencePayload</span></span>|<span data-ttu-id="16730-137">Stream</span><span class="sxs-lookup"><span data-stu-id="16730-137">Stream</span></span>|<span data-ttu-id="16730-138">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-139">полиципайлоад</span><span class="sxs-lookup"><span data-stu-id="16730-139">policyPayload</span></span>|<span data-ttu-id="16730-140">Stream</span><span class="sxs-lookup"><span data-stu-id="16730-140">Stream</span></span>|<span data-ttu-id="16730-141">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-142">description</span><span class="sxs-lookup"><span data-stu-id="16730-142">description</span></span>|<span data-ttu-id="16730-143">String</span><span class="sxs-lookup"><span data-stu-id="16730-143">String</span></span>|<span data-ttu-id="16730-144">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-145">displayName</span><span class="sxs-lookup"><span data-stu-id="16730-145">displayName</span></span>|<span data-ttu-id="16730-146">Строка</span><span class="sxs-lookup"><span data-stu-id="16730-146">String</span></span>|<span data-ttu-id="16730-147">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-148">priority</span><span class="sxs-lookup"><span data-stu-id="16730-148">priority</span></span>|<span data-ttu-id="16730-149">Int32</span><span class="sxs-lookup"><span data-stu-id="16730-149">Int32</span></span>|<span data-ttu-id="16730-150">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-151">усерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="16730-151">userCheckinSummary</span></span>|[<span data-ttu-id="16730-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="16730-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="16730-153">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="16730-154">чеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="16730-154">checkinStatuses</span></span>|<span data-ttu-id="16730-155">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="16730-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="16730-156">Еще не задокументировано, унаследовано от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16730-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="16730-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="16730-157">Response</span></span>
<span data-ttu-id="16730-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16730-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16730-159">Пример</span><span class="sxs-lookup"><span data-stu-id="16730-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="16730-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="16730-160">Request</span></span>
<span data-ttu-id="16730-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16730-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16730-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="16730-162">Response</span></span>
<span data-ttu-id="16730-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16730-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



