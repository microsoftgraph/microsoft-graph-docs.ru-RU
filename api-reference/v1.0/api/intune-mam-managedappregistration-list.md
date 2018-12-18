---
title: Перечисление объектов managedAppRegistration
description: Список свойств и связей объектов managedAppRegistration.
author: tfitzmac
ms.openlocfilehash: f51cea4eb5881e8a6d75a60b5877bf1175673e21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332237"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="31807-103">Перечисление объектов managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="31807-103">List managedAppRegistrations</span></span>

> <span data-ttu-id="31807-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="31807-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31807-105">Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="31807-105">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31807-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="31807-106">Prerequisites</span></span>
<span data-ttu-id="31807-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31807-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31807-109">Permission type</span></span>|<span data-ttu-id="31807-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31807-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31807-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31807-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31807-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="31807-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="31807-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31807-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31807-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31807-114">Not supported.</span></span>|
|<span data-ttu-id="31807-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31807-115">Application</span></span>|<span data-ttu-id="31807-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31807-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31807-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31807-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="31807-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31807-118">Request headers</span></span>
|<span data-ttu-id="31807-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31807-119">Header</span></span>|<span data-ttu-id="31807-120">Значение</span><span class="sxs-lookup"><span data-stu-id="31807-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31807-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31807-121">Authorization</span></span>|<span data-ttu-id="31807-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="31807-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31807-123">Accept</span><span class="sxs-lookup"><span data-stu-id="31807-123">Accept</span></span>|<span data-ttu-id="31807-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31807-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31807-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31807-125">Request body</span></span>
<span data-ttu-id="31807-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31807-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31807-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="31807-127">Response</span></span>
<span data-ttu-id="31807-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31807-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31807-129">Пример</span><span class="sxs-lookup"><span data-stu-id="31807-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="31807-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="31807-130">Request</span></span>
<span data-ttu-id="31807-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31807-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="31807-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="31807-132">Response</span></span>
<span data-ttu-id="31807-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="31807-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 806

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



