---
title: Получение iosVppAppAssignedDeviceLicense
description: Чтение свойства и связи объекта iosVppAppAssignedDeviceLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a8d41ea263682919d718531d7fdd53726ff867c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990224"
---
# <a name="get-iosvppappassigneddevicelicense"></a><span data-ttu-id="4f8fa-103">Получение iosVppAppAssignedDeviceLicense</span><span class="sxs-lookup"><span data-stu-id="4f8fa-103">Get iosVppAppAssignedDeviceLicense</span></span>

> <span data-ttu-id="4f8fa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f8fa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f8fa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f8fa-107">Чтение свойства и связи объекта [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="4f8fa-107">Read properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f8fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f8fa-108">Prerequisites</span></span>
<span data-ttu-id="4f8fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f8fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f8fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f8fa-111">Permission type</span></span>|<span data-ttu-id="4f8fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f8fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f8fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f8fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f8fa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f8fa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4f8fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f8fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f8fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-116">Not supported.</span></span>|
|<span data-ttu-id="4f8fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f8fa-117">Application</span></span>|<span data-ttu-id="4f8fa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f8fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f8fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f8fa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f8fa-120">Optional query parameters</span></span>
<span data-ttu-id="4f8fa-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f8fa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f8fa-122">Request headers</span></span>
|<span data-ttu-id="4f8fa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f8fa-123">Header</span></span>|<span data-ttu-id="4f8fa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4f8fa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f8fa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f8fa-125">Authorization</span></span>|<span data-ttu-id="4f8fa-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4f8fa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f8fa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4f8fa-127">Accept</span></span>|<span data-ttu-id="4f8fa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f8fa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f8fa-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f8fa-129">Request body</span></span>
<span data-ttu-id="4f8fa-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f8fa-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f8fa-131">Response</span></span>
<span data-ttu-id="4f8fa-132">Успешно завершена, этот метод возвращает `200 OK` объект [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-132">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f8fa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4f8fa-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f8fa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f8fa-134">Request</span></span>
<span data-ttu-id="4f8fa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="4f8fa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f8fa-136">Response</span></span>
<span data-ttu-id="4f8fa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f8fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
    "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "managedDeviceId": "Managed Device Id value",
    "deviceName": "Device Name value"
  }
}
```





