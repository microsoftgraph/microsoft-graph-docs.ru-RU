---
title: Get iosVppAppAssignedLicense
description: Чтение свойств и связей объекта iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dab6278dfabe22ed411fcfdf847c9096f75639e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143999"
---
# <a name="get-iosvppappassignedlicense"></a><span data-ttu-id="fcbf9-103">Get iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="fcbf9-103">Get iosVppAppAssignedLicense</span></span>

<span data-ttu-id="fcbf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcbf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcbf9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcbf9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcbf9-107">Чтение свойств и связей объекта [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="fcbf9-107">Read properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcbf9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fcbf9-108">Prerequisites</span></span>
<span data-ttu-id="fcbf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcbf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcbf9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcbf9-111">Permission type</span></span>|<span data-ttu-id="fcbf9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcbf9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcbf9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcbf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcbf9-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcbf9-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcbf9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcbf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcbf9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-116">Not supported.</span></span>|
|<span data-ttu-id="fcbf9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fcbf9-117">Application</span></span>|<span data-ttu-id="fcbf9-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcbf9-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcbf9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcbf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcbf9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcbf9-120">Optional query parameters</span></span>
<span data-ttu-id="fcbf9-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcbf9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcbf9-122">Request headers</span></span>
|<span data-ttu-id="fcbf9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcbf9-123">Header</span></span>|<span data-ttu-id="fcbf9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fcbf9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcbf9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcbf9-125">Authorization</span></span>|<span data-ttu-id="fcbf9-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcbf9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fcbf9-127">Accept</span></span>|<span data-ttu-id="fcbf9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fcbf9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcbf9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcbf9-129">Request body</span></span>
<span data-ttu-id="fcbf9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcbf9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcbf9-131">Response</span></span>
<span data-ttu-id="fcbf9-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-132">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcbf9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fcbf9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcbf9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcbf9-134">Request</span></span>
<span data-ttu-id="fcbf9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="fcbf9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcbf9-136">Response</span></span>
<span data-ttu-id="fcbf9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcbf9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 314

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
    "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```




