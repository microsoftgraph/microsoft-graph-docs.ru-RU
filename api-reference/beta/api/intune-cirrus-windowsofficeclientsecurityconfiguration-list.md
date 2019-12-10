---
title: Список Виндовсоффицеклиентсекуритиконфигуратионс
description: Список свойств и связей объектов Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88f134d9e5230d02b7be6fc92db8af78d839ae85
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39929911"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="c7075-103">Список Виндовсоффицеклиентсекуритиконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="c7075-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="c7075-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7075-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7075-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7075-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7075-106">Список свойств и связей объектов [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c7075-106">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7075-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7075-107">Prerequisites</span></span>
<span data-ttu-id="c7075-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7075-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7075-110">Permission type</span></span>|<span data-ttu-id="c7075-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7075-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7075-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7075-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7075-113">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c7075-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7075-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7075-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7075-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7075-115">Not supported.</span></span>|
|<span data-ttu-id="c7075-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7075-116">Application</span></span>|<span data-ttu-id="c7075-117">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c7075-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7075-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7075-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7075-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7075-119">Request headers</span></span>
|<span data-ttu-id="c7075-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7075-120">Header</span></span>|<span data-ttu-id="c7075-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c7075-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7075-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7075-122">Authorization</span></span>|<span data-ttu-id="c7075-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7075-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7075-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c7075-124">Accept</span></span>|<span data-ttu-id="c7075-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7075-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7075-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7075-126">Request body</span></span>
<span data-ttu-id="c7075-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7075-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7075-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7075-128">Response</span></span>
<span data-ttu-id="c7075-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7075-129">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7075-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c7075-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7075-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7075-131">Request</span></span>
<span data-ttu-id="c7075-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7075-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="c7075-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7075-133">Response</span></span>
<span data-ttu-id="c7075-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7075-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





