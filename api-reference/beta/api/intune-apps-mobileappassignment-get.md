---
title: Get mobileAppAssignment
description: Чтение свойств и связей объекта mobileAppAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a198f6c93edf79bdb2bbe156af6f80b5548f9c10
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935332"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="5b8ed-103">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="5b8ed-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="5b8ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b8ed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b8ed-106">Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5b8ed-106">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b8ed-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5b8ed-107">Prerequisites</span></span>
<span data-ttu-id="5b8ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b8ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b8ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b8ed-110">Permission type</span></span>|<span data-ttu-id="5b8ed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b8ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b8ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b8ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b8ed-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b8ed-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b8ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b8ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b8ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-115">Not supported.</span></span>|
|<span data-ttu-id="5b8ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b8ed-116">Application</span></span>|<span data-ttu-id="5b8ed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b8ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b8ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b8ed-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b8ed-119">Optional query parameters</span></span>
<span data-ttu-id="5b8ed-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b8ed-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b8ed-121">Request headers</span></span>
|<span data-ttu-id="5b8ed-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b8ed-122">Header</span></span>|<span data-ttu-id="5b8ed-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5b8ed-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b8ed-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b8ed-124">Authorization</span></span>|<span data-ttu-id="5b8ed-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b8ed-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5b8ed-126">Accept</span></span>|<span data-ttu-id="5b8ed-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5b8ed-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b8ed-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b8ed-128">Request body</span></span>
<span data-ttu-id="5b8ed-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b8ed-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b8ed-130">Response</span></span>
<span data-ttu-id="5b8ed-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-131">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b8ed-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5b8ed-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b8ed-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b8ed-133">Request</span></span>
<span data-ttu-id="5b8ed-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5b8ed-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b8ed-135">Response</span></span>
<span data-ttu-id="5b8ed-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b8ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "settings": {
      "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
    }
  }
}
```




