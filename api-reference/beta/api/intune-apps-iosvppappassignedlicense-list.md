---
title: Список iosVppAppAssignedLicenses
description: Свойства списка и связей объектов iosVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b02e35b7f0d2a6f64c2e1e891db6a6ae066be90b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883216"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="cd440-103">Список iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="cd440-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="cd440-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd440-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd440-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd440-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd440-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cd440-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd440-107">Свойства списка и связей объектов [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="cd440-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd440-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cd440-108">Prerequisites</span></span>
<span data-ttu-id="cd440-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd440-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd440-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd440-111">Permission type</span></span>|<span data-ttu-id="cd440-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd440-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd440-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd440-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd440-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd440-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cd440-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd440-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd440-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd440-116">Not supported.</span></span>|
|<span data-ttu-id="cd440-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd440-117">Application</span></span>|<span data-ttu-id="cd440-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd440-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd440-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd440-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="cd440-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd440-120">Request headers</span></span>
|<span data-ttu-id="cd440-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd440-121">Header</span></span>|<span data-ttu-id="cd440-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cd440-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd440-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd440-123">Authorization</span></span>|<span data-ttu-id="cd440-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cd440-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd440-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cd440-125">Accept</span></span>|<span data-ttu-id="cd440-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd440-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd440-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd440-127">Request body</span></span>
<span data-ttu-id="cd440-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd440-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd440-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd440-129">Response</span></span>
<span data-ttu-id="cd440-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cd440-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd440-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cd440-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd440-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd440-132">Request</span></span>
<span data-ttu-id="cd440-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd440-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="cd440-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd440-134">Response</span></span>
<span data-ttu-id="cd440-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cd440-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
      "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





