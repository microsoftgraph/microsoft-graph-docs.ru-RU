---
title: Перечисление объектов iosVppEBookAssignment
description: Список свойств и связей объектов iosVppEBookAssignment.
ms.openlocfilehash: f6e03361a3413c772517ab92deed6e7c9dc2322b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024687"
---
# <a name="list-iosvppebookassignments"></a><span data-ttu-id="4ee49-103">Перечисление объектов iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4ee49-103">List iosVppEBookAssignments</span></span>

> <span data-ttu-id="4ee49-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4ee49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ee49-105">Список свойств и связей объектов [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4ee49-105">List properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ee49-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4ee49-106">Prerequisites</span></span>
<span data-ttu-id="4ee49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ee49-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee49-109">Permission type</span></span>|<span data-ttu-id="4ee49-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ee49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ee49-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ee49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ee49-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ee49-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4ee49-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ee49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ee49-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee49-114">Not supported.</span></span>|
|<span data-ttu-id="4ee49-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ee49-115">Application</span></span>|<span data-ttu-id="4ee49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ee49-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ee49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4ee49-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ee49-118">Request headers</span></span>
|<span data-ttu-id="4ee49-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ee49-119">Header</span></span>|<span data-ttu-id="4ee49-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4ee49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ee49-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ee49-121">Authorization</span></span>|<span data-ttu-id="4ee49-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4ee49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ee49-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4ee49-123">Accept</span></span>|<span data-ttu-id="4ee49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4ee49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ee49-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ee49-125">Request body</span></span>
<span data-ttu-id="4ee49-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ee49-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ee49-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ee49-127">Response</span></span>
<span data-ttu-id="4ee49-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ee49-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ee49-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4ee49-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ee49-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ee49-130">Request</span></span>
<span data-ttu-id="4ee49-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ee49-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="4ee49-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ee49-132">Response</span></span>
<span data-ttu-id="4ee49-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4ee49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
      "id": "48f05789-5789-48f0-8957-f0488957f048",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```



