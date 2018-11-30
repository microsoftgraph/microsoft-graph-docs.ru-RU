---
title: Получение mobileAppInstallStatus
description: Чтение свойства и связи объекта mobileAppInstallStatus.
ms.openlocfilehash: 0663b3cb13714be201fd9f6917a2a0689d84402b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082271"
---
# <a name="get-mobileappinstallstatus"></a><span data-ttu-id="525d5-103">Получение mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="525d5-103">Get mobileAppInstallStatus</span></span>

> <span data-ttu-id="525d5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="525d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="525d5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="525d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="525d5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="525d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="525d5-107">Чтение свойства и связи объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="525d5-107">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="525d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="525d5-108">Prerequisites</span></span>
<span data-ttu-id="525d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="525d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="525d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="525d5-111">Permission type</span></span>|<span data-ttu-id="525d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="525d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="525d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="525d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="525d5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="525d5-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="525d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="525d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="525d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="525d5-116">Not supported.</span></span>|
|<span data-ttu-id="525d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="525d5-117">Application</span></span>|<span data-ttu-id="525d5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="525d5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="525d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="525d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="525d5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="525d5-120">Optional query parameters</span></span>
<span data-ttu-id="525d5-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="525d5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="525d5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="525d5-122">Request headers</span></span>
|<span data-ttu-id="525d5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="525d5-123">Header</span></span>|<span data-ttu-id="525d5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="525d5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="525d5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="525d5-125">Authorization</span></span>|<span data-ttu-id="525d5-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="525d5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="525d5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="525d5-127">Accept</span></span>|<span data-ttu-id="525d5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="525d5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="525d5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="525d5-129">Request body</span></span>
<span data-ttu-id="525d5-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="525d5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="525d5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="525d5-131">Response</span></span>
<span data-ttu-id="525d5-132">Успешно завершена, этот метод возвращает `200 OK` объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="525d5-132">If successful, this method returns a `200 OK` response code and [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="525d5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="525d5-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="525d5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="525d5-134">Request</span></span>
<span data-ttu-id="525d5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="525d5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="525d5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="525d5-136">Response</span></span>
<span data-ttu-id="525d5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="525d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
    "id": "7560ee45-ee45-7560-45ee-607545ee6075",
    "deviceName": "Device Name value",
    "deviceId": "Device Id value",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "mobileAppInstallStatusValue": "failed",
    "installState": "failed",
    "installStateDetail": "seeInstallErrorCode",
    "errorCode": 9,
    "osVersion": "Os Version value",
    "osDescription": "Os Description value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "displayVersion": "Display Version value"
  }
}
```





