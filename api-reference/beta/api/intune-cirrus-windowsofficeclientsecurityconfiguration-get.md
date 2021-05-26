---
title: Получить windowsOfficeClientSecurityConfiguration
description: Получите определенный объект политики безопасности windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adaad0a5a43e415a17c21218272b98afe3a502ec
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667019"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="5bbb1-103">Получить windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="5bbb1-103">Get windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="5bbb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bbb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bbb1-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bbb1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bbb1-107">Получите определенный объект [политики безопасности windowsOfficeClientSecurityConfiguration.](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5bbb1-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bbb1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5bbb1-108">Prerequisites</span></span>
<span data-ttu-id="5bbb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bbb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bbb1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bbb1-111">Permission type</span></span>|<span data-ttu-id="5bbb1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bbb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bbb1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bbb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bbb1-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bbb1-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5bbb1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bbb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bbb1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-116">Not supported.</span></span>|
|<span data-ttu-id="5bbb1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5bbb1-117">Application</span></span>|<span data-ttu-id="5bbb1-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bbb1-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bbb1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bbb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bbb1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5bbb1-120">Optional query parameters</span></span>
<span data-ttu-id="5bbb1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bbb1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bbb1-122">Request headers</span></span>
|<span data-ttu-id="5bbb1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bbb1-123">Header</span></span>|<span data-ttu-id="5bbb1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5bbb1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bbb1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bbb1-125">Authorization</span></span>|<span data-ttu-id="5bbb1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bbb1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5bbb1-127">Accept</span></span>|<span data-ttu-id="5bbb1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5bbb1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bbb1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bbb1-129">Request body</span></span>
<span data-ttu-id="5bbb1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bbb1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbb1-131">Response</span></span>
<span data-ttu-id="5bbb1-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект WindowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bbb1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5bbb1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bbb1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbb1-134">Request</span></span>
<span data-ttu-id="5bbb1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="5bbb1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbb1-136">Response</span></span>
<span data-ttu-id="5bbb1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": {
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
}
```




