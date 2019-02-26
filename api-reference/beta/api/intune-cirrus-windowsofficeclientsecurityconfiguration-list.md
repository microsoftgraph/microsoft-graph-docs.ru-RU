---
title: Список Виндовсоффицеклиентсекуритиконфигуратионс
description: Список свойств и связей объектов Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e97b364e7a30a85bd5b9109dd41806b7ed8589a4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145390"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="15270-103">Список Виндовсоффицеклиентсекуритиконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="15270-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="15270-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15270-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15270-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15270-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15270-106">Список свойств и связей объектов [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15270-106">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15270-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15270-107">Prerequisites</span></span>
<span data-ttu-id="15270-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15270-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15270-110">Permission type</span></span>|<span data-ttu-id="15270-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15270-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15270-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15270-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15270-113">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="15270-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="15270-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15270-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15270-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15270-115">Not supported.</span></span>|
|<span data-ttu-id="15270-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15270-116">Application</span></span>|<span data-ttu-id="15270-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15270-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15270-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15270-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15270-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15270-119">Request headers</span></span>
|<span data-ttu-id="15270-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15270-120">Header</span></span>|<span data-ttu-id="15270-121">Значение</span><span class="sxs-lookup"><span data-stu-id="15270-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15270-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15270-122">Authorization</span></span>|<span data-ttu-id="15270-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="15270-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15270-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15270-124">Accept</span></span>|<span data-ttu-id="15270-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15270-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15270-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15270-126">Request body</span></span>
<span data-ttu-id="15270-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15270-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15270-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="15270-128">Response</span></span>
<span data-ttu-id="15270-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15270-129">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15270-130">Пример</span><span class="sxs-lookup"><span data-stu-id="15270-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="15270-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="15270-131">Request</span></span>
<span data-ttu-id="15270-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15270-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="15270-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="15270-133">Response</span></span>
<span data-ttu-id="15270-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15270-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "value": [
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
  ]
}
```



