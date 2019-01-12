---
title: Перечисление объектов managedAppRegistration
description: Список свойств и связей объектов managedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a52b9930862450efc872457984241384443ac0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955998"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="79ede-103">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="79ede-103">List managedAppRegistrations</span></span>

> <span data-ttu-id="79ede-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79ede-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79ede-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ede-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79ede-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79ede-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79ede-107">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="79ede-107">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79ede-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79ede-108">Prerequisites</span></span>
<span data-ttu-id="79ede-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79ede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79ede-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79ede-111">Permission type</span></span>|<span data-ttu-id="79ede-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79ede-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79ede-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79ede-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79ede-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79ede-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="79ede-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79ede-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79ede-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ede-116">Not supported.</span></span>|
|<span data-ttu-id="79ede-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79ede-117">Application</span></span>|<span data-ttu-id="79ede-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ede-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79ede-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79ede-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="79ede-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79ede-120">Request headers</span></span>
|<span data-ttu-id="79ede-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79ede-121">Header</span></span>|<span data-ttu-id="79ede-122">Значение</span><span class="sxs-lookup"><span data-stu-id="79ede-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79ede-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ede-123">Authorization</span></span>|<span data-ttu-id="79ede-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="79ede-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79ede-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79ede-125">Accept</span></span>|<span data-ttu-id="79ede-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79ede-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ede-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79ede-127">Request body</span></span>
<span data-ttu-id="79ede-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79ede-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79ede-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ede-129">Response</span></span>
<span data-ttu-id="79ede-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="79ede-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79ede-131">Пример</span><span class="sxs-lookup"><span data-stu-id="79ede-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="79ede-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="79ede-132">Request</span></span>
<span data-ttu-id="79ede-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79ede-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="79ede-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="79ede-134">Response</span></span>
<span data-ttu-id="79ede-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79ede-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1014

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
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
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```





