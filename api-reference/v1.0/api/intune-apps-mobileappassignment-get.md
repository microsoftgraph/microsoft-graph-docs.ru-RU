---
title: Get mobileAppAssignment
description: Чтение свойств и связей объекта mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29306173db3a037ed455adc8b6ab0992a717360f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016127"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="0ee6a-103">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="0ee6a-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="0ee6a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee6a-105">Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0ee6a-105">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee6a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee6a-106">Prerequisites</span></span>
<span data-ttu-id="0ee6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee6a-109">Permission type</span></span>|<span data-ttu-id="0ee6a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ee6a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ee6a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee6a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee6a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0ee6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ee6a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee6a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-114">Not supported.</span></span>|
|<span data-ttu-id="0ee6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ee6a-115">Application</span></span>|<span data-ttu-id="0ee6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ee6a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ee6a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ee6a-118">Optional query parameters</span></span>
<span data-ttu-id="0ee6a-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ee6a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ee6a-120">Request headers</span></span>
|<span data-ttu-id="0ee6a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ee6a-121">Header</span></span>|<span data-ttu-id="0ee6a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ee6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee6a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ee6a-123">Authorization</span></span>|<span data-ttu-id="0ee6a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee6a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ee6a-125">Accept</span></span>|<span data-ttu-id="0ee6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee6a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ee6a-127">Request body</span></span>
<span data-ttu-id="0ee6a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee6a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ee6a-129">Response</span></span>
<span data-ttu-id="0ee6a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-130">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee6a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ee6a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee6a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ee6a-132">Request</span></span>
<span data-ttu-id="0ee6a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0ee6a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee6a-134">Response</span></span>
<span data-ttu-id="0ee6a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ee6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



