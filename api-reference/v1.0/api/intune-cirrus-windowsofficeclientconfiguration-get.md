---
title: Получить windowsOfficeClientConfiguration
description: Получите определенный объект политики безопасности windowsOfficeClientConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53238bdb656967ccc3e230532270057d1cb5f07c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751989"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="9e0be-103">Получить windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e0be-103">Get windowsOfficeClientConfiguration</span></span>

<span data-ttu-id="9e0be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e0be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e0be-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e0be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e0be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e0be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e0be-107">Получите определенный объект политики безопасности [windowsOfficeClientConfiguration.](../resources/intune-cirrus-windowsofficeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e0be-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e0be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9e0be-108">Prerequisites</span></span>
<span data-ttu-id="9e0be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e0be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e0be-111">Permission type</span></span>|<span data-ttu-id="9e0be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e0be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e0be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e0be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e0be-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e0be-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e0be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e0be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e0be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e0be-116">Not supported.</span></span>|
|<span data-ttu-id="9e0be-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e0be-117">Application</span></span>|<span data-ttu-id="9e0be-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e0be-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e0be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e0be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e0be-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e0be-120">Optional query parameters</span></span>
<span data-ttu-id="9e0be-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e0be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e0be-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e0be-122">Request headers</span></span>
|<span data-ttu-id="9e0be-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e0be-123">Header</span></span>|<span data-ttu-id="9e0be-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9e0be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e0be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e0be-125">Authorization</span></span>|<span data-ttu-id="9e0be-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e0be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e0be-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9e0be-127">Accept</span></span>|<span data-ttu-id="9e0be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9e0be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e0be-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e0be-129">Request body</span></span>
<span data-ttu-id="9e0be-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e0be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e0be-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e0be-131">Response</span></span>
<span data-ttu-id="9e0be-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e0be-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e0be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9e0be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e0be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e0be-134">Request</span></span>
<span data-ttu-id="9e0be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e0be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="9e0be-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e0be-136">Response</span></span>
<span data-ttu-id="9e0be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e0be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
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
}
```




