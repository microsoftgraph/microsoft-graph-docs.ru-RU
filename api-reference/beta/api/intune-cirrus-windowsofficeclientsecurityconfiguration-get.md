---
title: Получение Виндовсоффицеклиентсекуритиконфигуратион
description: Получение определенного объекта политики безопасности Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02edba061958739dd0dac43151e027b414be19d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152167"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="b408d-103">Получение Виндовсоффицеклиентсекуритиконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b408d-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="b408d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b408d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b408d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b408d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b408d-106">Получение определенного объекта политики безопасности [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b408d-106">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b408d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b408d-107">Prerequisites</span></span>
<span data-ttu-id="b408d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b408d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b408d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b408d-110">Permission type</span></span>|<span data-ttu-id="b408d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b408d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b408d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b408d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b408d-113">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b408d-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b408d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b408d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b408d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b408d-115">Not supported.</span></span>|
|<span data-ttu-id="b408d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b408d-116">Application</span></span>|<span data-ttu-id="b408d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b408d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b408d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b408d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b408d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b408d-119">Optional query parameters</span></span>
<span data-ttu-id="b408d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b408d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b408d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b408d-121">Request headers</span></span>
|<span data-ttu-id="b408d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b408d-122">Header</span></span>|<span data-ttu-id="b408d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b408d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b408d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b408d-124">Authorization</span></span>|<span data-ttu-id="b408d-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b408d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b408d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b408d-126">Accept</span></span>|<span data-ttu-id="b408d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b408d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b408d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b408d-128">Request body</span></span>
<span data-ttu-id="b408d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b408d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b408d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b408d-130">Response</span></span>
<span data-ttu-id="b408d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b408d-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b408d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b408d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b408d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b408d-133">Request</span></span>
<span data-ttu-id="b408d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b408d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="b408d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b408d-135">Response</span></span>
<span data-ttu-id="b408d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b408d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



