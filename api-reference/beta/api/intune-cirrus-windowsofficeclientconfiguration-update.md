---
title: Обновление windowsOfficeClientConfiguration
description: Исправление полезных определенной политики не связанные с безопасностью.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e13228c6fc467fa49b740c02b4b7068efb1ec42e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863877"
---
# <a name="update-windowsofficeclientconfiguration"></a><span data-ttu-id="3cc79-103">Обновление windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="3cc79-103">Update windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="3cc79-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3cc79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3cc79-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cc79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cc79-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3cc79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cc79-107">Исправление полезных определенной политики не связанные с безопасностью.</span><span class="sxs-lookup"><span data-stu-id="3cc79-107">Patch a specific non-security policy payload.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cc79-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3cc79-108">Prerequisites</span></span>
<span data-ttu-id="3cc79-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cc79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc79-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cc79-111">Permission type</span></span>|<span data-ttu-id="3cc79-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cc79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cc79-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cc79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3cc79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cc79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cc79-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cc79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cc79-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cc79-116">Not supported.</span></span>|
|<span data-ttu-id="3cc79-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cc79-117">Application</span></span>|<span data-ttu-id="3cc79-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cc79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cc79-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cc79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="3cc79-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cc79-120">Request headers</span></span>
|<span data-ttu-id="3cc79-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cc79-121">Header</span></span>|<span data-ttu-id="3cc79-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3cc79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cc79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cc79-123">Authorization</span></span>|<span data-ttu-id="3cc79-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3cc79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cc79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3cc79-125">Accept</span></span>|<span data-ttu-id="3cc79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3cc79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cc79-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3cc79-127">Request body</span></span>
<span data-ttu-id="3cc79-128">В тексте запроса укажите представление JSON для объекта [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3cc79-128">In the request body, supply a JSON representation for the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

<span data-ttu-id="3cc79-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3cc79-129">The following table shows the properties that are required when you create the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md).</span></span>

|<span data-ttu-id="3cc79-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cc79-130">Property</span></span>|<span data-ttu-id="3cc79-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3cc79-131">Type</span></span>|<span data-ttu-id="3cc79-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3cc79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc79-133">id</span><span class="sxs-lookup"><span data-stu-id="3cc79-133">id</span></span>|<span data-ttu-id="3cc79-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3cc79-134">String</span></span>|<span data-ttu-id="3cc79-135">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-135">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-136">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="3cc79-136">userPreferencePayload</span></span>|<span data-ttu-id="3cc79-137">Stream</span><span class="sxs-lookup"><span data-stu-id="3cc79-137">Stream</span></span>|<span data-ttu-id="3cc79-138">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-138">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-139">policyPayload</span><span class="sxs-lookup"><span data-stu-id="3cc79-139">policyPayload</span></span>|<span data-ttu-id="3cc79-140">Stream</span><span class="sxs-lookup"><span data-stu-id="3cc79-140">Stream</span></span>|<span data-ttu-id="3cc79-141">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-141">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-142">описание</span><span class="sxs-lookup"><span data-stu-id="3cc79-142">description</span></span>|<span data-ttu-id="3cc79-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3cc79-143">String</span></span>|<span data-ttu-id="3cc79-144">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-144">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-145">displayName</span><span class="sxs-lookup"><span data-stu-id="3cc79-145">displayName</span></span>|<span data-ttu-id="3cc79-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3cc79-146">String</span></span>|<span data-ttu-id="3cc79-147">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-147">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-148">priority</span><span class="sxs-lookup"><span data-stu-id="3cc79-148">priority</span></span>|<span data-ttu-id="3cc79-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3cc79-149">Int32</span></span>|<span data-ttu-id="3cc79-150">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-150">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-151">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3cc79-151">userCheckinSummary</span></span>|[<span data-ttu-id="3cc79-152">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="3cc79-152">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="3cc79-153">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-153">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|
|<span data-ttu-id="3cc79-154">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="3cc79-154">checkinStatuses</span></span>|<span data-ttu-id="3cc79-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3cc79-155">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="3cc79-156">Еще не описываются Inherited с [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cc79-156">Not yet documented Inherited from [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3cc79-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cc79-157">Response</span></span>
<span data-ttu-id="3cc79-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3cc79-158">If successful, this method returns a `200 OK` response code and an updated [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cc79-159">Пример</span><span class="sxs-lookup"><span data-stu-id="3cc79-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cc79-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cc79-160">Request</span></span>
<span data-ttu-id="3cc79-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cc79-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3cc79-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cc79-162">Response</span></span>
<span data-ttu-id="3cc79-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3cc79-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



