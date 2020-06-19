---
title: Get iosVppEBookAssignment
description: Чтение свойств и связей объекта iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f982e4d54cff8e71f79b1b62c07c9f76af7297c4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793236"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="0c755-103">Get iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="0c755-103">Get iosVppEBookAssignment</span></span>

<span data-ttu-id="0c755-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c755-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c755-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c755-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c755-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c755-107">Чтение свойств и связей объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0c755-107">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c755-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0c755-108">Prerequisites</span></span>
<span data-ttu-id="0c755-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0c755-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0c755-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c755-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c755-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c755-111">Permission type</span></span>|<span data-ttu-id="0c755-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c755-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c755-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c755-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c755-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c755-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0c755-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c755-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c755-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c755-116">Not supported.</span></span>|
|<span data-ttu-id="0c755-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c755-117">Application</span></span>|<span data-ttu-id="0c755-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c755-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c755-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c755-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c755-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0c755-120">Optional query parameters</span></span>
<span data-ttu-id="0c755-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c755-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c755-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c755-122">Request headers</span></span>
|<span data-ttu-id="0c755-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c755-123">Header</span></span>|<span data-ttu-id="0c755-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0c755-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c755-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c755-125">Authorization</span></span>|<span data-ttu-id="0c755-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c755-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c755-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0c755-127">Accept</span></span>|<span data-ttu-id="0c755-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0c755-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c755-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c755-129">Request body</span></span>
<span data-ttu-id="0c755-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c755-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c755-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c755-131">Response</span></span>
<span data-ttu-id="0c755-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c755-132">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c755-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0c755-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c755-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c755-134">Request</span></span>
<span data-ttu-id="0c755-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c755-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="0c755-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c755-136">Response</span></span>
<span data-ttu-id="0c755-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="0c755-137">Here is an example of the response.</span></span> <span data-ttu-id="0c755-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="0c755-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0c755-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0c755-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 444

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
    "id": "48f05789-5789-48f0-8957-f0488957f048",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "installIntent": "required"
  }
}
```



