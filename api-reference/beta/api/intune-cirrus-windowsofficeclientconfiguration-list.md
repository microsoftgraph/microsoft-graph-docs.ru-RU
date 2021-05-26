---
title: Список windowsOfficeClientConfigurations
description: Список свойств и связей объектов WindowsOfficeClientConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf9582fc12a83df2dcc4e49a429a8df9e807dea7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665897"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="626ba-103">Список windowsOfficeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="626ba-103">List windowsOfficeClientConfigurations</span></span>

<span data-ttu-id="626ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="626ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="626ba-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="626ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="626ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="626ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="626ba-107">Список свойств и связей [объектов WindowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="626ba-107">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="626ba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="626ba-108">Prerequisites</span></span>
<span data-ttu-id="626ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="626ba-111">Permission type</span></span>|<span data-ttu-id="626ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="626ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="626ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="626ba-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="626ba-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="626ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="626ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="626ba-116">Not supported.</span></span>|
|<span data-ttu-id="626ba-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="626ba-117">Application</span></span>|<span data-ttu-id="626ba-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="626ba-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="626ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="626ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="626ba-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="626ba-120">Request headers</span></span>
|<span data-ttu-id="626ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="626ba-121">Header</span></span>|<span data-ttu-id="626ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="626ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="626ba-123">Authorization</span></span>|<span data-ttu-id="626ba-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="626ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="626ba-125">Accept</span></span>|<span data-ttu-id="626ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="626ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="626ba-127">Request body</span></span>
<span data-ttu-id="626ba-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="626ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="626ba-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="626ba-129">Response</span></span>
<span data-ttu-id="626ba-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="626ba-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="626ba-131">Пример</span><span class="sxs-lookup"><span data-stu-id="626ba-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="626ba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="626ba-132">Request</span></span>
<span data-ttu-id="626ba-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="626ba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="626ba-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="626ba-134">Response</span></span>
<span data-ttu-id="626ba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="626ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1214

{
  "value": [
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
  ]
}
```




