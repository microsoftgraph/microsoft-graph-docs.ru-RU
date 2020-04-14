---
title: Получение officeClientConfiguration
description: Получение определенной политики.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 235e2b498b788d15268de197364442d8f7bb75e1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392171"
---
# <a name="get-officeclientconfiguration"></a><span data-ttu-id="a35be-103">Получение officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="a35be-103">Get officeClientConfiguration</span></span>

<span data-ttu-id="a35be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a35be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a35be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a35be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a35be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a35be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a35be-107">Получение определенной политики.</span><span class="sxs-lookup"><span data-stu-id="a35be-107">Get a specific policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a35be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a35be-108">Prerequisites</span></span>
<span data-ttu-id="a35be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a35be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a35be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a35be-111">Permission type</span></span>|<span data-ttu-id="a35be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a35be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a35be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a35be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a35be-114">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a35be-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a35be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a35be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a35be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a35be-116">Not supported.</span></span>|
|<span data-ttu-id="a35be-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a35be-117">Application</span></span>|<span data-ttu-id="a35be-118">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a35be-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a35be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a35be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a35be-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a35be-120">Optional query parameters</span></span>
<span data-ttu-id="a35be-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a35be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a35be-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a35be-122">Request headers</span></span>
|<span data-ttu-id="a35be-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a35be-123">Header</span></span>|<span data-ttu-id="a35be-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a35be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a35be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a35be-125">Authorization</span></span>|<span data-ttu-id="a35be-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a35be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a35be-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a35be-127">Accept</span></span>|<span data-ttu-id="a35be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a35be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a35be-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a35be-129">Request body</span></span>
<span data-ttu-id="a35be-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a35be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a35be-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a35be-131">Response</span></span>
<span data-ttu-id="a35be-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a35be-132">If successful, this method returns a `200 OK` response code and [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a35be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a35be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a35be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a35be-134">Request</span></span>
<span data-ttu-id="a35be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a35be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="a35be-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a35be-136">Response</span></span>
<span data-ttu-id="a35be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a35be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfiguration",
    "id": "362ce0f0-e0f0-362c-f0e0-2c36f0e02c36",
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



