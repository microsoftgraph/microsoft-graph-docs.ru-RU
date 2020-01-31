---
title: Получение Манажеддевицемобилеаппконфигуратионстате
description: Чтение свойств и связей объекта Манажеддевицемобилеаппконфигуратионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d83f3f1a011ad772f2b62914adb42a77c48ce87
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636324"
---
# <a name="get-manageddevicemobileappconfigurationstate"></a><span data-ttu-id="40b3d-103">Получение Манажеддевицемобилеаппконфигуратионстате</span><span class="sxs-lookup"><span data-stu-id="40b3d-103">Get managedDeviceMobileAppConfigurationState</span></span>

> <span data-ttu-id="40b3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40b3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40b3d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40b3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40b3d-106">Чтение свойств и связей объекта Манажеддевицемобилеаппконфигуратионстате.</span><span class="sxs-lookup"><span data-stu-id="40b3d-106">Read properties and relationships of the managedDeviceMobileAppConfigurationState object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40b3d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="40b3d-107">Prerequisites</span></span>
<span data-ttu-id="40b3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40b3d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40b3d-110">Permission type</span></span>|<span data-ttu-id="40b3d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40b3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40b3d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40b3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40b3d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40b3d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40b3d-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40b3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40b3d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40b3d-115">Not supported.</span></span>|
|<span data-ttu-id="40b3d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40b3d-116">Application</span></span>|<span data-ttu-id="40b3d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40b3d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40b3d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40b3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40b3d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40b3d-119">Optional query parameters</span></span>
<span data-ttu-id="40b3d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="40b3d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40b3d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40b3d-121">Request headers</span></span>
|<span data-ttu-id="40b3d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40b3d-122">Header</span></span>|<span data-ttu-id="40b3d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="40b3d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40b3d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40b3d-124">Authorization</span></span>|<span data-ttu-id="40b3d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40b3d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40b3d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="40b3d-126">Accept</span></span>|<span data-ttu-id="40b3d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40b3d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40b3d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40b3d-128">Request body</span></span>
<span data-ttu-id="40b3d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40b3d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40b3d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="40b3d-130">Response</span></span>
<span data-ttu-id="40b3d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект манажеддевицемобилеаппконфигуратионстате в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40b3d-131">If successful, this method returns a `200 OK` response code and managedDeviceMobileAppConfigurationState object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40b3d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="40b3d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="40b3d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="40b3d-133">Request</span></span>
<span data-ttu-id="40b3d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40b3d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
```

### <a name="response"></a><span data-ttu-id="40b3d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40b3d-135">Response</span></span>
<span data-ttu-id="40b3d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40b3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1225

{
  "value": {
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
}
```



