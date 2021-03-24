---
title: Список iosVppAppAssignedLicenses
description: Список свойств и связей объектов iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11acb03c0155a5baf5a4f185ab5322b2b8b02983
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140569"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="d708d-103">Список iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="d708d-103">List iosVppAppAssignedLicenses</span></span>

<span data-ttu-id="d708d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d708d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d708d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d708d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d708d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d708d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d708d-107">Список свойств и связей объектов [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d708d-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d708d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d708d-108">Prerequisites</span></span>
<span data-ttu-id="d708d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d708d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d708d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d708d-111">Permission type</span></span>|<span data-ttu-id="d708d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d708d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d708d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d708d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d708d-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d708d-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d708d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d708d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d708d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d708d-116">Not supported.</span></span>|
|<span data-ttu-id="d708d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d708d-117">Application</span></span>|<span data-ttu-id="d708d-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d708d-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d708d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d708d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="d708d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d708d-120">Request headers</span></span>
|<span data-ttu-id="d708d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d708d-121">Header</span></span>|<span data-ttu-id="d708d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d708d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d708d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d708d-123">Authorization</span></span>|<span data-ttu-id="d708d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d708d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d708d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d708d-125">Accept</span></span>|<span data-ttu-id="d708d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d708d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d708d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d708d-127">Request body</span></span>
<span data-ttu-id="d708d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d708d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d708d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d708d-129">Response</span></span>
<span data-ttu-id="d708d-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d708d-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d708d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d708d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d708d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d708d-132">Request</span></span>
<span data-ttu-id="d708d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d708d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="d708d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d708d-134">Response</span></span>
<span data-ttu-id="d708d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d708d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




