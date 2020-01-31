---
title: Список Манажеддевицемобилеаппконфигуратионстатес
description: Список свойств и связей объектов Манажеддевицемобилеаппконфигуратионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78b247c403a8cea0594cb30e1210f55f1cdf0ddc
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636323"
---
# <a name="list-manageddevicemobileappconfigurationstates"></a><span data-ttu-id="90a01-103">Список Манажеддевицемобилеаппконфигуратионстатес</span><span class="sxs-lookup"><span data-stu-id="90a01-103">List managedDeviceMobileAppConfigurationStates</span></span>

> <span data-ttu-id="90a01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90a01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90a01-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90a01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90a01-106">Список свойств и связей объектов Манажеддевицемобилеаппконфигуратионстате.</span><span class="sxs-lookup"><span data-stu-id="90a01-106">List properties and relationships of the managedDeviceMobileAppConfigurationState objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90a01-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90a01-107">Prerequisites</span></span>
<span data-ttu-id="90a01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90a01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90a01-110">Permission type</span></span>|<span data-ttu-id="90a01-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90a01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90a01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90a01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90a01-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90a01-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90a01-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90a01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90a01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90a01-115">Not supported.</span></span>|
|<span data-ttu-id="90a01-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90a01-116">Application</span></span>|<span data-ttu-id="90a01-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90a01-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90a01-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90a01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
```

## <a name="request-headers"></a><span data-ttu-id="90a01-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90a01-119">Request headers</span></span>
|<span data-ttu-id="90a01-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90a01-120">Header</span></span>|<span data-ttu-id="90a01-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90a01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90a01-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90a01-122">Authorization</span></span>|<span data-ttu-id="90a01-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90a01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90a01-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90a01-124">Accept</span></span>|<span data-ttu-id="90a01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90a01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90a01-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90a01-126">Request body</span></span>
<span data-ttu-id="90a01-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90a01-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90a01-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="90a01-128">Response</span></span>
<span data-ttu-id="90a01-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов манажеддевицемобилеаппконфигуратионстате в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90a01-129">If successful, this method returns a `200 OK` response code and a collection of managedDeviceMobileAppConfigurationState objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90a01-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90a01-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90a01-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90a01-131">Request</span></span>
<span data-ttu-id="90a01-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90a01-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
```

### <a name="response"></a><span data-ttu-id="90a01-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="90a01-133">Response</span></span>
<span data-ttu-id="90a01-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90a01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
      "id": "659554f2-54f2-6595-f254-9565f2549565",
      "settingStates": [
        {
          "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
          "setting": "Setting value",
          "settingName": "Setting Name value",
          "instanceDisplayName": "Instance Display Name value",
          "state": "notApplicable",
          "errorCode": 9,
          "errorDescription": "Error Description value",
          "userId": "User Id value",
          "userName": "User Name value",
          "userEmail": "User Email value",
          "userPrincipalName": "User Principal Name value",
          "sources": [
            {
              "@odata.type": "microsoft.graph.settingSource",
              "id": "Id value",
              "displayName": "Display Name value"
            }
          ],
          "currentValue": "Current Value value"
        }
      ],
      "displayName": "Display Name value",
      "version": 7,
      "platformType": "androidForWork",
      "state": "notApplicable",
      "settingCount": 12,
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



