---
title: Список Рестриктедаппсвиолатионс
description: Список свойств и связей объектов Рестриктедаппсвиолатион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a66a87f30c815c45d9d8f39b44bd8409eb57705
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172109"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="89993-103">Список Рестриктедаппсвиолатионс</span><span class="sxs-lookup"><span data-stu-id="89993-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="89993-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89993-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89993-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89993-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89993-106">Список свойств и связей объектов [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="89993-106">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89993-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89993-107">Prerequisites</span></span>
<span data-ttu-id="89993-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="89993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="89993-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89993-110">Permission type</span></span>|<span data-ttu-id="89993-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89993-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89993-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89993-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89993-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89993-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89993-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89993-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89993-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89993-115">Not supported.</span></span>|
|<span data-ttu-id="89993-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89993-116">Application</span></span>|<span data-ttu-id="89993-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89993-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89993-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89993-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="89993-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89993-119">Request headers</span></span>
|<span data-ttu-id="89993-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89993-120">Header</span></span>|<span data-ttu-id="89993-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89993-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89993-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89993-122">Authorization</span></span>|<span data-ttu-id="89993-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="89993-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89993-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89993-124">Accept</span></span>|<span data-ttu-id="89993-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89993-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89993-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89993-126">Request body</span></span>
<span data-ttu-id="89993-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89993-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89993-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="89993-128">Response</span></span>
<span data-ttu-id="89993-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89993-129">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89993-130">Пример</span><span class="sxs-lookup"><span data-stu-id="89993-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="89993-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="89993-131">Request</span></span>
<span data-ttu-id="89993-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89993-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="89993-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="89993-133">Response</span></span>
<span data-ttu-id="89993-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89993-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




