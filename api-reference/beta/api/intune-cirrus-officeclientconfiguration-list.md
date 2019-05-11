---
title: Список Оффицеклиентконфигуратионс
description: Получить все политики.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 093364b093606153fd82c18791a86ff441291d56
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934070"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="36355-103">Список Оффицеклиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="36355-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="36355-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36355-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36355-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36355-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36355-106">Получить все политики.</span><span class="sxs-lookup"><span data-stu-id="36355-106">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36355-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36355-107">Prerequisites</span></span>
<span data-ttu-id="36355-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36355-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36355-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36355-110">Permission type</span></span>|<span data-ttu-id="36355-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36355-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36355-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36355-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36355-113">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="36355-113">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36355-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36355-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36355-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36355-115">Not supported.</span></span>|
|<span data-ttu-id="36355-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36355-116">Application</span></span>|<span data-ttu-id="36355-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36355-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36355-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36355-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="36355-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36355-119">Request headers</span></span>
|<span data-ttu-id="36355-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36355-120">Header</span></span>|<span data-ttu-id="36355-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36355-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36355-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36355-122">Authorization</span></span>|<span data-ttu-id="36355-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36355-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36355-124">Accept</span><span class="sxs-lookup"><span data-stu-id="36355-124">Accept</span></span>|<span data-ttu-id="36355-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36355-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36355-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36355-126">Request body</span></span>
<span data-ttu-id="36355-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36355-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36355-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="36355-128">Response</span></span>
<span data-ttu-id="36355-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36355-129">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36355-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36355-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="36355-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36355-131">Request</span></span>
<span data-ttu-id="36355-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36355-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="36355-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="36355-133">Response</span></span>
<span data-ttu-id="36355-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36355-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1207

{
  "value": [
    {
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
  ]
}
```



