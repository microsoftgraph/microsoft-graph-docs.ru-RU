---
title: Список iosVppAppAssignedUserLicenses
description: Свойства списка и связей объектов iosVppAppAssignedUserLicense.
ms.openlocfilehash: 7ab7b55dfdcd9f8cbe2d015f46ac013e7840db26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081205"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="1629e-103">Список iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="1629e-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="1629e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1629e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1629e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1629e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1629e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1629e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1629e-107">Свойства списка и связей объектов [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1629e-107">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1629e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1629e-108">Prerequisites</span></span>
<span data-ttu-id="1629e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1629e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1629e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1629e-111">Permission type</span></span>|<span data-ttu-id="1629e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1629e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1629e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1629e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1629e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1629e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1629e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1629e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1629e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1629e-116">Not supported.</span></span>|
|<span data-ttu-id="1629e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1629e-117">Application</span></span>|<span data-ttu-id="1629e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1629e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1629e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1629e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="1629e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1629e-120">Request headers</span></span>
|<span data-ttu-id="1629e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1629e-121">Header</span></span>|<span data-ttu-id="1629e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1629e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1629e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1629e-123">Authorization</span></span>|<span data-ttu-id="1629e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1629e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1629e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1629e-125">Accept</span></span>|<span data-ttu-id="1629e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1629e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1629e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1629e-127">Request body</span></span>
<span data-ttu-id="1629e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1629e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1629e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1629e-129">Response</span></span>
<span data-ttu-id="1629e-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1629e-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1629e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1629e-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1629e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1629e-132">Request</span></span>
<span data-ttu-id="1629e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1629e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="1629e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1629e-134">Response</span></span>
<span data-ttu-id="1629e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1629e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
      "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





