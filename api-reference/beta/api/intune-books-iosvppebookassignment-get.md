---
title: Get iosVppEBookAssignment
description: Чтение свойств и связей объекта iosVppEBookAssignment.
ms.openlocfilehash: ef3432164899f639a6865cd0219189e15d55a6cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080113"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="8638a-103">Get iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="8638a-103">Get iosVppEBookAssignment</span></span>

> <span data-ttu-id="8638a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8638a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8638a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8638a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8638a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8638a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8638a-107">Чтение свойств и связей объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8638a-107">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8638a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8638a-108">Prerequisites</span></span>
<span data-ttu-id="8638a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8638a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8638a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8638a-111">Permission type</span></span>|<span data-ttu-id="8638a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8638a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8638a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8638a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8638a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8638a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8638a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8638a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8638a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8638a-116">Not supported.</span></span>|
|<span data-ttu-id="8638a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8638a-117">Application</span></span>|<span data-ttu-id="8638a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8638a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8638a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8638a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8638a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8638a-120">Optional query parameters</span></span>
<span data-ttu-id="8638a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8638a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8638a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8638a-122">Request headers</span></span>
|<span data-ttu-id="8638a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8638a-123">Header</span></span>|<span data-ttu-id="8638a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8638a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8638a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8638a-125">Authorization</span></span>|<span data-ttu-id="8638a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8638a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8638a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8638a-127">Accept</span></span>|<span data-ttu-id="8638a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8638a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8638a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8638a-129">Request body</span></span>
<span data-ttu-id="8638a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8638a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8638a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8638a-131">Response</span></span>
<span data-ttu-id="8638a-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8638a-132">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8638a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8638a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8638a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8638a-134">Request</span></span>
<span data-ttu-id="8638a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8638a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="8638a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8638a-136">Response</span></span>
<span data-ttu-id="8638a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8638a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





