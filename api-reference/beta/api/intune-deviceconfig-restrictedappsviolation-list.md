---
title: Список Рестриктедаппсвиолатионс
description: Список свойств и связей объектов Рестриктедаппсвиолатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 136736c07302bc1741084662dfa33539b77ef587
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947836"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="5a806-103">Список Рестриктедаппсвиолатионс</span><span class="sxs-lookup"><span data-stu-id="5a806-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="5a806-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a806-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a806-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a806-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a806-106">Список свойств и связей объектов [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="5a806-106">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a806-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a806-107">Prerequisites</span></span>
<span data-ttu-id="5a806-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a806-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a806-110">Permission type</span></span>|<span data-ttu-id="5a806-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a806-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a806-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a806-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a806-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a806-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a806-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a806-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a806-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a806-115">Not supported.</span></span>|
|<span data-ttu-id="5a806-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a806-116">Application</span></span>|<span data-ttu-id="5a806-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a806-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a806-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a806-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="5a806-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5a806-119">Request headers</span></span>
|<span data-ttu-id="5a806-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a806-120">Header</span></span>|<span data-ttu-id="5a806-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a806-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a806-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a806-122">Authorization</span></span>|<span data-ttu-id="5a806-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a806-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a806-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a806-124">Accept</span></span>|<span data-ttu-id="5a806-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a806-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a806-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a806-126">Request body</span></span>
<span data-ttu-id="5a806-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a806-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a806-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a806-128">Response</span></span>
<span data-ttu-id="5a806-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a806-129">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a806-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5a806-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a806-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a806-131">Request</span></span>
<span data-ttu-id="5a806-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a806-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="5a806-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a806-133">Response</span></span>
<span data-ttu-id="5a806-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a806-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 710

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "53f99903-9903-53f9-0399-f9530399f953",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "androidForWork",
      "restrictedAppsState": "notApprovedApps",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```





