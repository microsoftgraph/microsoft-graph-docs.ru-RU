---
title: Get iosVppEBookAssignment
description: Чтение свойств и связей объекта iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ec822e57d951a496f846d21f02186c8cad1f743
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148036"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="d6d39-103">Get iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="d6d39-103">Get iosVppEBookAssignment</span></span>

> <span data-ttu-id="d6d39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6d39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d39-106">Чтение свойств и связей объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d6d39-106">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d39-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d6d39-107">Prerequisites</span></span>
<span data-ttu-id="d6d39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6d39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d6d39-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6d39-110">Permission type</span></span>|<span data-ttu-id="d6d39-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6d39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d39-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6d39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d39-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6d39-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d6d39-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6d39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d39-115">Not supported.</span></span>|
|<span data-ttu-id="d6d39-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6d39-116">Application</span></span>|<span data-ttu-id="d6d39-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d39-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6d39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6d39-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6d39-119">Optional query parameters</span></span>
<span data-ttu-id="d6d39-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6d39-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6d39-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6d39-121">Request headers</span></span>
|<span data-ttu-id="d6d39-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6d39-122">Header</span></span>|<span data-ttu-id="d6d39-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d6d39-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d39-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6d39-124">Authorization</span></span>|<span data-ttu-id="d6d39-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d6d39-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d39-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d6d39-126">Accept</span></span>|<span data-ttu-id="d6d39-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d39-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d39-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6d39-128">Request body</span></span>
<span data-ttu-id="d6d39-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6d39-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6d39-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6d39-130">Response</span></span>
<span data-ttu-id="d6d39-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d6d39-131">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d39-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d6d39-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d39-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6d39-133">Request</span></span>
<span data-ttu-id="d6d39-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6d39-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d6d39-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6d39-135">Response</span></span>
<span data-ttu-id="d6d39-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6d39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




