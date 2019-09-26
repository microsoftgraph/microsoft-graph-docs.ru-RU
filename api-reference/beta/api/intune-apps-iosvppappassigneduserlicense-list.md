---
title: Список Иосвппаппассигнедусерлиценсес
description: Список свойств и связей объектов Иосвппаппассигнедусерлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fc806ef8bf344e9ef441877fff4060f44f89076
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173418"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="0e3d6-103">Список Иосвппаппассигнедусерлиценсес</span><span class="sxs-lookup"><span data-stu-id="0e3d6-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="0e3d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e3d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e3d6-106">Список свойств и связей объектов [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0e3d6-106">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e3d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e3d6-107">Prerequisites</span></span>
<span data-ttu-id="0e3d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e3d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e3d6-110">Permission type</span></span>|<span data-ttu-id="0e3d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e3d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e3d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e3d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e3d6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e3d6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0e3d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e3d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e3d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-115">Not supported.</span></span>|
|<span data-ttu-id="0e3d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e3d6-116">Application</span></span>|<span data-ttu-id="0e3d6-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e3d6-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e3d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e3d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="0e3d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e3d6-119">Request headers</span></span>
|<span data-ttu-id="0e3d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e3d6-120">Header</span></span>|<span data-ttu-id="0e3d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e3d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e3d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e3d6-122">Authorization</span></span>|<span data-ttu-id="0e3d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e3d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e3d6-124">Accept</span></span>|<span data-ttu-id="0e3d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e3d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e3d6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e3d6-126">Request body</span></span>
<span data-ttu-id="0e3d6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e3d6-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e3d6-128">Response</span></span>
<span data-ttu-id="0e3d6-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e3d6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0e3d6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e3d6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e3d6-131">Request</span></span>
<span data-ttu-id="0e3d6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="0e3d6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e3d6-133">Response</span></span>
<span data-ttu-id="0e3d6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e3d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




