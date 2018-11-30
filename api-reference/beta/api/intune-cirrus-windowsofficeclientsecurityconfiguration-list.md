---
title: Список windowsOfficeClientSecurityConfigurations
description: Свойства списка и связей объектов windowsOfficeClientSecurityConfiguration.
ms.openlocfilehash: 281a910658100b990b988b462b46984534cb2cbe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082463"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a><span data-ttu-id="78566-103">Список windowsOfficeClientSecurityConfigurations</span><span class="sxs-lookup"><span data-stu-id="78566-103">List windowsOfficeClientSecurityConfigurations</span></span>

> <span data-ttu-id="78566-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78566-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78566-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78566-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78566-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78566-107">Свойства списка и связей объектов [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="78566-107">List properties and relationships of the [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78566-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78566-108">Prerequisites</span></span>
<span data-ttu-id="78566-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78566-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78566-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78566-111">Permission type</span></span>|<span data-ttu-id="78566-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78566-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78566-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78566-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78566-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78566-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78566-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78566-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78566-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78566-116">Not supported.</span></span>|
|<span data-ttu-id="78566-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78566-117">Application</span></span>|<span data-ttu-id="78566-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78566-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78566-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78566-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="78566-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78566-120">Request headers</span></span>
|<span data-ttu-id="78566-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78566-121">Header</span></span>|<span data-ttu-id="78566-122">Значение</span><span class="sxs-lookup"><span data-stu-id="78566-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78566-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78566-123">Authorization</span></span>|<span data-ttu-id="78566-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="78566-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78566-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78566-125">Accept</span></span>|<span data-ttu-id="78566-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78566-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78566-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78566-127">Request body</span></span>
<span data-ttu-id="78566-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78566-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78566-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="78566-129">Response</span></span>
<span data-ttu-id="78566-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="78566-130">If successful, this method returns a `200 OK` response code and a collection of [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78566-131">Пример</span><span class="sxs-lookup"><span data-stu-id="78566-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="78566-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="78566-132">Request</span></span>
<span data-ttu-id="78566-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78566-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="78566-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="78566-134">Response</span></span>
<span data-ttu-id="78566-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="78566-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



