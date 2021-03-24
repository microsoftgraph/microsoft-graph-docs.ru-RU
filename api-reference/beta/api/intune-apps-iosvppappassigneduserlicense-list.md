---
title: Список iosVppAppAssignedUserLicenses
description: Список свойств и связей объектов iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3277091c14b6764596b8c60bead43ecd937c0dc8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144006"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="0c0d7-103">Список iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="0c0d7-103">List iosVppAppAssignedUserLicenses</span></span>

<span data-ttu-id="0c0d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c0d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c0d7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c0d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c0d7-107">Список свойств и связей объектов [iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0c0d7-107">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c0d7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c0d7-108">Prerequisites</span></span>
<span data-ttu-id="0c0d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c0d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c0d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c0d7-111">Permission type</span></span>|<span data-ttu-id="0c0d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c0d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c0d7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c0d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c0d7-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0d7-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c0d7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c0d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c0d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-116">Not supported.</span></span>|
|<span data-ttu-id="0c0d7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c0d7-117">Application</span></span>|<span data-ttu-id="0c0d7-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0d7-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c0d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c0d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="0c0d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c0d7-120">Request headers</span></span>
|<span data-ttu-id="0c0d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c0d7-121">Header</span></span>|<span data-ttu-id="0c0d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c0d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c0d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c0d7-123">Authorization</span></span>|<span data-ttu-id="0c0d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c0d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c0d7-125">Accept</span></span>|<span data-ttu-id="0c0d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c0d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c0d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c0d7-127">Request body</span></span>
<span data-ttu-id="0c0d7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c0d7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c0d7-129">Response</span></span>
<span data-ttu-id="0c0d7-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c0d7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0c0d7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c0d7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c0d7-132">Request</span></span>
<span data-ttu-id="0c0d7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="0c0d7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c0d7-134">Response</span></span>
<span data-ttu-id="0c0d7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c0d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




