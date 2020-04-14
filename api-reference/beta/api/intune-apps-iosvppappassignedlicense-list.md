---
title: Список Иосвппаппассигнедлиценсес
description: Список свойств и связей объектов Иосвппаппассигнедлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc1e0371634d6c48f54666d608c91b9101718676
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416618"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="2b344-103">Список Иосвппаппассигнедлиценсес</span><span class="sxs-lookup"><span data-stu-id="2b344-103">List iosVppAppAssignedLicenses</span></span>

<span data-ttu-id="2b344-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b344-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b344-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b344-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b344-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b344-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b344-107">Список свойств и связей объектов [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="2b344-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b344-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b344-108">Prerequisites</span></span>
<span data-ttu-id="2b344-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b344-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b344-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b344-111">Permission type</span></span>|<span data-ttu-id="2b344-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b344-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b344-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b344-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b344-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b344-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2b344-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b344-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b344-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b344-116">Not supported.</span></span>|
|<span data-ttu-id="2b344-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b344-117">Application</span></span>|<span data-ttu-id="2b344-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b344-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b344-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b344-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="2b344-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b344-120">Request headers</span></span>
|<span data-ttu-id="2b344-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b344-121">Header</span></span>|<span data-ttu-id="2b344-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b344-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b344-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b344-123">Authorization</span></span>|<span data-ttu-id="2b344-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b344-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b344-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b344-125">Accept</span></span>|<span data-ttu-id="2b344-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b344-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b344-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b344-127">Request body</span></span>
<span data-ttu-id="2b344-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b344-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b344-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b344-129">Response</span></span>
<span data-ttu-id="2b344-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b344-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b344-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2b344-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b344-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b344-132">Request</span></span>
<span data-ttu-id="2b344-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b344-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="2b344-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b344-134">Response</span></span>
<span data-ttu-id="2b344-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b344-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



