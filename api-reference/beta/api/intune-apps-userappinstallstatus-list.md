---
title: Список userAppInstallStatuses
description: Свойства списка и связей объектов userAppInstallStatus.
ms.openlocfilehash: 86bb3bc288a2890635e5ad676358b09c3c91ccb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082625"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="4c324-103">Список userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="4c324-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="4c324-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c324-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c324-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c324-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c324-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c324-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c324-107">Свойства списка и связей объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="4c324-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c324-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c324-108">Prerequisites</span></span>
<span data-ttu-id="4c324-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c324-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c324-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c324-111">Permission type</span></span>|<span data-ttu-id="4c324-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c324-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c324-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c324-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c324-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4c324-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c324-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c324-116">Not supported.</span></span>|
|<span data-ttu-id="4c324-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c324-117">Application</span></span>|<span data-ttu-id="4c324-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c324-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c324-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4c324-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c324-120">Request headers</span></span>
|<span data-ttu-id="4c324-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c324-121">Header</span></span>|<span data-ttu-id="4c324-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c324-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c324-123">Authorization</span></span>|<span data-ttu-id="4c324-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c324-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c324-125">Accept</span></span>|<span data-ttu-id="4c324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c324-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c324-127">Request body</span></span>
<span data-ttu-id="4c324-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c324-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c324-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c324-129">Response</span></span>
<span data-ttu-id="4c324-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4c324-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c324-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4c324-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c324-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c324-132">Request</span></span>
<span data-ttu-id="4c324-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c324-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="4c324-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c324-134">Response</span></span>
<span data-ttu-id="4c324-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4c324-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```





