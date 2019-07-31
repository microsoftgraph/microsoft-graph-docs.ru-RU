---
title: Получение Иосвппаппассигнедлиценсе
description: Чтение свойств и связей объекта Иосвппаппассигнедлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59b7f812e0e55fa117d17b7ac663c2ad64d7d75c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962346"
---
# <a name="get-iosvppappassignedlicense"></a><span data-ttu-id="fa942-103">Получение Иосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="fa942-103">Get iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="fa942-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa942-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa942-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa942-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa942-106">Чтение свойств и связей объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="fa942-106">Read properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa942-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa942-107">Prerequisites</span></span>
<span data-ttu-id="fa942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa942-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa942-110">Permission type</span></span>|<span data-ttu-id="fa942-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa942-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa942-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa942-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa942-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa942-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa942-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa942-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa942-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa942-115">Not supported.</span></span>|
|<span data-ttu-id="fa942-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa942-116">Application</span></span>|<span data-ttu-id="fa942-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa942-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa942-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa942-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa942-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa942-119">Optional query parameters</span></span>
<span data-ttu-id="fa942-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa942-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa942-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa942-121">Request headers</span></span>
|<span data-ttu-id="fa942-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa942-122">Header</span></span>|<span data-ttu-id="fa942-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fa942-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa942-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa942-124">Authorization</span></span>|<span data-ttu-id="fa942-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa942-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa942-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fa942-126">Accept</span></span>|<span data-ttu-id="fa942-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fa942-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa942-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa942-128">Request body</span></span>
<span data-ttu-id="fa942-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa942-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa942-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa942-130">Response</span></span>
<span data-ttu-id="fa942-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa942-131">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa942-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fa942-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa942-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa942-133">Request</span></span>
<span data-ttu-id="fa942-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa942-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="fa942-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa942-135">Response</span></span>
<span data-ttu-id="fa942-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





