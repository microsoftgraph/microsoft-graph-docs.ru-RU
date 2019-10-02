---
title: Get iosVppEBookAssignment
description: Чтение свойств и связей объекта iosVppEBookAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73ab7989849f4208616966fec66960c436ffad1a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357901"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="d3879-103">Get iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="d3879-103">Get iosVppEBookAssignment</span></span>

> <span data-ttu-id="d3879-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3879-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3879-105">Чтение свойств и связей объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d3879-105">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3879-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d3879-106">Prerequisites</span></span>
<span data-ttu-id="d3879-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3879-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3879-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3879-109">Permission type</span></span>|<span data-ttu-id="d3879-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3879-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3879-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3879-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3879-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3879-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3879-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3879-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3879-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3879-114">Not supported.</span></span>|
|<span data-ttu-id="d3879-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3879-115">Application</span></span>|<span data-ttu-id="d3879-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3879-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3879-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3879-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3879-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3879-118">Optional query parameters</span></span>
<span data-ttu-id="d3879-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d3879-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3879-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3879-120">Request headers</span></span>
|<span data-ttu-id="d3879-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3879-121">Header</span></span>|<span data-ttu-id="d3879-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3879-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3879-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3879-123">Authorization</span></span>|<span data-ttu-id="d3879-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3879-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3879-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3879-125">Accept</span></span>|<span data-ttu-id="d3879-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3879-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3879-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3879-127">Request body</span></span>
<span data-ttu-id="d3879-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3879-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3879-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3879-129">Response</span></span>
<span data-ttu-id="d3879-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d3879-130">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3879-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d3879-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3879-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3879-132">Request</span></span>
<span data-ttu-id="d3879-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3879-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d3879-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3879-134">Response</span></span>
<span data-ttu-id="d3879-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3879-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
    "id": "48f05789-5789-48f0-8957-f0488957f048",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```




