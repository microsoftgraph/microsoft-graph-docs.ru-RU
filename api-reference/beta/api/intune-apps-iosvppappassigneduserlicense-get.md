---
title: Получение Иосвппаппассигнедусерлиценсе
description: Чтение свойств и связей объекта Иосвппаппассигнедусерлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17db79b52a5cc96f46e37ee944c6bc7bb84fd35b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330316"
---
# <a name="get-iosvppappassigneduserlicense"></a><span data-ttu-id="69287-103">Получение Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="69287-103">Get iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="69287-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69287-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69287-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69287-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69287-106">Чтение свойств и связей объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="69287-106">Read properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69287-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69287-107">Prerequisites</span></span>
<span data-ttu-id="69287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69287-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69287-110">Permission type</span></span>|<span data-ttu-id="69287-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69287-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69287-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69287-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69287-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69287-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="69287-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69287-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69287-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69287-115">Not supported.</span></span>|
|<span data-ttu-id="69287-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69287-116">Application</span></span>|<span data-ttu-id="69287-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69287-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69287-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69287-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69287-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69287-119">Optional query parameters</span></span>
<span data-ttu-id="69287-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="69287-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69287-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69287-121">Request headers</span></span>
|<span data-ttu-id="69287-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69287-122">Header</span></span>|<span data-ttu-id="69287-123">Значение</span><span class="sxs-lookup"><span data-stu-id="69287-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69287-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69287-124">Authorization</span></span>|<span data-ttu-id="69287-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69287-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69287-126">Accept</span><span class="sxs-lookup"><span data-stu-id="69287-126">Accept</span></span>|<span data-ttu-id="69287-127">application/json</span><span class="sxs-lookup"><span data-stu-id="69287-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69287-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69287-128">Request body</span></span>
<span data-ttu-id="69287-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69287-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69287-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="69287-130">Response</span></span>
<span data-ttu-id="69287-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69287-131">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69287-132">Пример</span><span class="sxs-lookup"><span data-stu-id="69287-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="69287-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="69287-133">Request</span></span>
<span data-ttu-id="69287-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69287-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="69287-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="69287-135">Response</span></span>
<span data-ttu-id="69287-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
    "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```






