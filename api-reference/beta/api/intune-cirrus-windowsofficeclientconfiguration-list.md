---
title: Список Виндовсоффицеклиентконфигуратионс
description: Список свойств и связей объектов Виндовсоффицеклиентконфигуратион.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad44d265371bd7865d26fc3d38808ac568647248
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170758"
---
# <a name="list-windowsofficeclientconfigurations"></a><span data-ttu-id="de9a4-103">Список Виндовсоффицеклиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="de9a4-103">List windowsOfficeClientConfigurations</span></span>

> <span data-ttu-id="de9a4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de9a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de9a4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de9a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de9a4-106">Список свойств и связей объектов [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="de9a4-106">List properties and relationships of the [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de9a4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de9a4-107">Prerequisites</span></span>
<span data-ttu-id="de9a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de9a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de9a4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de9a4-110">Permission type</span></span>|<span data-ttu-id="de9a4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de9a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de9a4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de9a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de9a4-113">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="de9a4-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="de9a4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de9a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de9a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de9a4-115">Not supported.</span></span>|
|<span data-ttu-id="de9a4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de9a4-116">Application</span></span>|<span data-ttu-id="de9a4-117">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="de9a4-117">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de9a4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de9a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de9a4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de9a4-119">Request headers</span></span>
|<span data-ttu-id="de9a4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de9a4-120">Header</span></span>|<span data-ttu-id="de9a4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de9a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de9a4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de9a4-122">Authorization</span></span>|<span data-ttu-id="de9a4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de9a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de9a4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de9a4-124">Accept</span></span>|<span data-ttu-id="de9a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de9a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de9a4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de9a4-126">Request body</span></span>
<span data-ttu-id="de9a4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de9a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de9a4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="de9a4-128">Response</span></span>
<span data-ttu-id="de9a4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de9a4-129">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de9a4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="de9a4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="de9a4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="de9a4-131">Request</span></span>
<span data-ttu-id="de9a4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de9a4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="de9a4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="de9a4-133">Response</span></span>
<span data-ttu-id="de9a4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de9a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




