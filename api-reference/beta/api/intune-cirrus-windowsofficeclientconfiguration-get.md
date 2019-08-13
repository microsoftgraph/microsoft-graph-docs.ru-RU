---
title: Получение Виндовсоффицеклиентконфигуратион
description: Получение определенного объекта Виндовсоффицеклиентконфигуратион политики, не относящейся к безопасности.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e1f34ead1df597a6b94df224398a6f6c2f77ab3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328230"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="849af-103">Получение Виндовсоффицеклиентконфигуратион</span><span class="sxs-lookup"><span data-stu-id="849af-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="849af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="849af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="849af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="849af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="849af-106">Получение определенного объекта [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) политики, не относящейся к безопасности.</span><span class="sxs-lookup"><span data-stu-id="849af-106">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="849af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="849af-107">Prerequisites</span></span>
<span data-ttu-id="849af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="849af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="849af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="849af-110">Permission type</span></span>|<span data-ttu-id="849af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="849af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="849af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="849af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="849af-113">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="849af-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="849af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="849af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="849af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="849af-115">Not supported.</span></span>|
|<span data-ttu-id="849af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="849af-116">Application</span></span>|<span data-ttu-id="849af-117">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="849af-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="849af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="849af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="849af-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="849af-119">Optional query parameters</span></span>
<span data-ttu-id="849af-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="849af-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="849af-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="849af-121">Request headers</span></span>
|<span data-ttu-id="849af-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="849af-122">Header</span></span>|<span data-ttu-id="849af-123">Значение</span><span class="sxs-lookup"><span data-stu-id="849af-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="849af-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="849af-124">Authorization</span></span>|<span data-ttu-id="849af-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="849af-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="849af-126">Accept</span><span class="sxs-lookup"><span data-stu-id="849af-126">Accept</span></span>|<span data-ttu-id="849af-127">application/json</span><span class="sxs-lookup"><span data-stu-id="849af-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="849af-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="849af-128">Request body</span></span>
<span data-ttu-id="849af-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="849af-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="849af-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="849af-130">Response</span></span>
<span data-ttu-id="849af-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="849af-131">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="849af-132">Пример</span><span class="sxs-lookup"><span data-stu-id="849af-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="849af-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="849af-133">Request</span></span>
<span data-ttu-id="849af-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="849af-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="849af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="849af-135">Response</span></span>
<span data-ttu-id="849af-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="849af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






