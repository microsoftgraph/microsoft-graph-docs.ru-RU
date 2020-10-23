---
title: Список Оффицеклиентконфигуратионс
description: Получить все политики.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b758166e557e24e888d975c8ca7ab943729b1eae
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690135"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="142f8-103">Список Оффицеклиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="142f8-103">List officeClientConfigurations</span></span>

<span data-ttu-id="142f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="142f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="142f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="142f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="142f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="142f8-107">Получить все политики.</span><span class="sxs-lookup"><span data-stu-id="142f8-107">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="142f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="142f8-108">Prerequisites</span></span>
<span data-ttu-id="142f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="142f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="142f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="142f8-111">Permission type</span></span>|<span data-ttu-id="142f8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="142f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="142f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="142f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="142f8-114">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="142f8-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="142f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="142f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="142f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="142f8-116">Not supported.</span></span>|
|<span data-ttu-id="142f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="142f8-117">Application</span></span>|<span data-ttu-id="142f8-118">DeviceManagementConfiguration. ReadWrite. ALL DeviceManagementConfiguration. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="142f8-118">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="142f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="142f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="142f8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="142f8-120">Request headers</span></span>
|<span data-ttu-id="142f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="142f8-121">Header</span></span>|<span data-ttu-id="142f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="142f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="142f8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="142f8-123">Authorization</span></span>|<span data-ttu-id="142f8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="142f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="142f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="142f8-125">Accept</span></span>|<span data-ttu-id="142f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="142f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="142f8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="142f8-127">Request body</span></span>
<span data-ttu-id="142f8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="142f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="142f8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="142f8-129">Response</span></span>
<span data-ttu-id="142f8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="142f8-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="142f8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="142f8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="142f8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="142f8-132">Request</span></span>
<span data-ttu-id="142f8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="142f8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="142f8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="142f8-134">Response</span></span>
<span data-ttu-id="142f8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="142f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





