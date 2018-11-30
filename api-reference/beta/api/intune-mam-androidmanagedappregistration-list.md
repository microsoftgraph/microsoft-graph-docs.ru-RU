---
title: Перечисление объектов androidManagedAppRegistration
description: Список свойств и связей объектов androidManagedAppRegistration.
ms.openlocfilehash: 208faffd512cfa517a999e6f3c043e1bc637a8e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082191"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="6de78-103">Перечисление объектов androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="6de78-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="6de78-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6de78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6de78-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6de78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6de78-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6de78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6de78-107">Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="6de78-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6de78-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6de78-108">Prerequisites</span></span>
<span data-ttu-id="6de78-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6de78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6de78-111">Permission type</span></span>|<span data-ttu-id="6de78-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6de78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6de78-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6de78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6de78-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6de78-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6de78-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6de78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6de78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6de78-116">Not supported.</span></span>|
|<span data-ttu-id="6de78-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6de78-117">Application</span></span>|<span data-ttu-id="6de78-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6de78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6de78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6de78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="6de78-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6de78-120">Request headers</span></span>
|<span data-ttu-id="6de78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6de78-121">Header</span></span>|<span data-ttu-id="6de78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6de78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6de78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6de78-123">Authorization</span></span>|<span data-ttu-id="6de78-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6de78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6de78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6de78-125">Accept</span></span>|<span data-ttu-id="6de78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6de78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6de78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6de78-127">Request body</span></span>
<span data-ttu-id="6de78-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6de78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6de78-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6de78-129">Response</span></span>
<span data-ttu-id="6de78-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6de78-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6de78-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6de78-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6de78-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6de78-132">Request</span></span>
<span data-ttu-id="6de78-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6de78-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="6de78-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6de78-134">Response</span></span>
<span data-ttu-id="6de78-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6de78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1070

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "managedDeviceId": "Managed Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```





