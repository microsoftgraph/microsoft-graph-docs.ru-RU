---
title: Получение Иосвппаппассигнедусерлиценсе
description: Чтение свойств и связей объекта Иосвппаппассигнедусерлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25dd4ead9f9c27274679557524402627bc00c482
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935995"
---
# <a name="get-iosvppappassigneduserlicense"></a><span data-ttu-id="28939-103">Получение Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="28939-103">Get iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="28939-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28939-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28939-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28939-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28939-106">Чтение свойств и связей объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="28939-106">Read properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28939-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28939-107">Prerequisites</span></span>
<span data-ttu-id="28939-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28939-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28939-110">Permission type</span></span>|<span data-ttu-id="28939-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28939-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28939-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28939-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28939-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28939-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="28939-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28939-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28939-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28939-115">Not supported.</span></span>|
|<span data-ttu-id="28939-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28939-116">Application</span></span>|<span data-ttu-id="28939-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28939-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28939-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28939-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28939-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28939-119">Optional query parameters</span></span>
<span data-ttu-id="28939-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="28939-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28939-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28939-121">Request headers</span></span>
|<span data-ttu-id="28939-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28939-122">Header</span></span>|<span data-ttu-id="28939-123">Значение</span><span class="sxs-lookup"><span data-stu-id="28939-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28939-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28939-124">Authorization</span></span>|<span data-ttu-id="28939-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28939-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28939-126">Accept</span><span class="sxs-lookup"><span data-stu-id="28939-126">Accept</span></span>|<span data-ttu-id="28939-127">application/json</span><span class="sxs-lookup"><span data-stu-id="28939-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28939-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28939-128">Request body</span></span>
<span data-ttu-id="28939-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28939-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28939-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="28939-130">Response</span></span>
<span data-ttu-id="28939-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28939-131">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28939-132">Пример</span><span class="sxs-lookup"><span data-stu-id="28939-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="28939-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="28939-133">Request</span></span>
<span data-ttu-id="28939-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28939-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="28939-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="28939-135">Response</span></span>
<span data-ttu-id="28939-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




