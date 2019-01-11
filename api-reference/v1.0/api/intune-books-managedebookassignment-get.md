---
title: Get managedEBookAssignment
description: Чтение свойств и связей объекта managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac7dc8a9caf9e346a0b71933fa0ffe17add6597a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821184"
---
# <a name="get-managedebookassignment"></a><span data-ttu-id="6e80a-103">Get managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="6e80a-103">Get managedEBookAssignment</span></span>

> <span data-ttu-id="6e80a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6e80a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e80a-105">Чтение свойств и связей объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6e80a-105">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e80a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6e80a-106">Prerequisites</span></span>
<span data-ttu-id="6e80a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e80a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e80a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e80a-109">Permission type</span></span>|<span data-ttu-id="6e80a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e80a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e80a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e80a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6e80a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e80a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6e80a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e80a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e80a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e80a-114">Not supported.</span></span>|
|<span data-ttu-id="6e80a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e80a-115">Application</span></span>|<span data-ttu-id="6e80a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e80a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e80a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e80a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e80a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e80a-118">Optional query parameters</span></span>
<span data-ttu-id="6e80a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6e80a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e80a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e80a-120">Request headers</span></span>
|<span data-ttu-id="6e80a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e80a-121">Header</span></span>|<span data-ttu-id="6e80a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e80a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e80a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e80a-123">Authorization</span></span>|<span data-ttu-id="6e80a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6e80a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e80a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e80a-125">Accept</span></span>|<span data-ttu-id="6e80a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e80a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e80a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6e80a-127">Request body</span></span>
<span data-ttu-id="6e80a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e80a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e80a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e80a-129">Response</span></span>
<span data-ttu-id="6e80a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e80a-130">If successful, this method returns a `200 OK` response code and [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e80a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6e80a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e80a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e80a-132">Request</span></span>
<span data-ttu-id="6e80a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e80a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6e80a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e80a-134">Response</span></span>
<span data-ttu-id="6e80a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6e80a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookAssignment",
    "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```



