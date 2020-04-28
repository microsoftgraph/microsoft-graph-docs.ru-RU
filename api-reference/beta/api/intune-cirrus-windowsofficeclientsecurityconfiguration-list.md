---
title: Список Виндовсоффицеклиентсекуритиконфигуратионс
description: Список свойств и связей объектов Виндовсоффицеклиентсекуритиконфигуратион.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c6c71222cad55f6353a7fbea4c0d73184041262
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436641"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="7baf3-103">Список Виндовсоффицеклиентсекуритиконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="7baf3-103">List windowsOfficeClientSecurityConfigurations</span></span>

<span data-ttu-id="7baf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7baf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7baf3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7baf3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7baf3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7baf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7baf3-107">Список свойств и связей объектов [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7baf3-107">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7baf3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7baf3-108">Prerequisites</span></span>
<span data-ttu-id="7baf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7baf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7baf3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7baf3-111">Permission type</span></span>|<span data-ttu-id="7baf3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7baf3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7baf3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7baf3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7baf3-114">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7baf3-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7baf3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7baf3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7baf3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7baf3-116">Not supported.</span></span>|
|<span data-ttu-id="7baf3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7baf3-117">Application</span></span>|<span data-ttu-id="7baf3-118">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7baf3-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7baf3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7baf3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7baf3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7baf3-120">Request headers</span></span>
|<span data-ttu-id="7baf3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7baf3-121">Header</span></span>|<span data-ttu-id="7baf3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7baf3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7baf3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7baf3-123">Authorization</span></span>|<span data-ttu-id="7baf3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7baf3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7baf3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7baf3-125">Accept</span></span>|<span data-ttu-id="7baf3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7baf3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7baf3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7baf3-127">Request body</span></span>
<span data-ttu-id="7baf3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7baf3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7baf3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7baf3-129">Response</span></span>
<span data-ttu-id="7baf3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсоффицеклиентсекуритиконфигуратион](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7baf3-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7baf3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7baf3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7baf3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7baf3-132">Request</span></span>
<span data-ttu-id="7baf3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7baf3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="7baf3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7baf3-134">Response</span></span>
<span data-ttu-id="7baf3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7baf3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



