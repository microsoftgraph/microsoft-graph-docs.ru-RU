---
title: Get mobileAppAssignment
description: Чтение свойств и связей объекта mobileAppAssignment.
ms.openlocfilehash: 4f27085439240b79ba77778893931872715c851f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027640"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="47284-103">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="47284-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="47284-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47284-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47284-105">Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47284-105">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47284-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="47284-106">Prerequisites</span></span>
<span data-ttu-id="47284-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47284-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47284-109">Permission type</span></span>|<span data-ttu-id="47284-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47284-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47284-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47284-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47284-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47284-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="47284-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47284-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47284-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47284-114">Not supported.</span></span>|
|<span data-ttu-id="47284-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47284-115">Application</span></span>|<span data-ttu-id="47284-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47284-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47284-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47284-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47284-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47284-118">Optional query parameters</span></span>
<span data-ttu-id="47284-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47284-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="47284-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47284-120">Request headers</span></span>
|<span data-ttu-id="47284-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47284-121">Header</span></span>|<span data-ttu-id="47284-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47284-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47284-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47284-123">Authorization</span></span>|<span data-ttu-id="47284-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47284-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47284-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47284-125">Accept</span></span>|<span data-ttu-id="47284-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47284-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47284-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47284-127">Request body</span></span>
<span data-ttu-id="47284-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47284-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47284-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="47284-129">Response</span></span>
<span data-ttu-id="47284-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47284-130">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47284-131">Пример</span><span class="sxs-lookup"><span data-stu-id="47284-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="47284-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="47284-132">Request</span></span>
<span data-ttu-id="47284-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47284-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="47284-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="47284-134">Response</span></span>
<span data-ttu-id="47284-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="47284-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



