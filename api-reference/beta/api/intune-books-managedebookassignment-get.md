---
title: Get managedEBookAssignment
description: Чтение свойств и связей объекта managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b4a1a29b8650d13992d63beb46de5e21f875ca6
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085101"
---
# <a name="get-managedebookassignment"></a><span data-ttu-id="c5f2d-103">Get managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="c5f2d-103">Get managedEBookAssignment</span></span>

> <span data-ttu-id="c5f2d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f2d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f2d-106">Чтение свойств и связей объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5f2d-106">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f2d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f2d-107">Prerequisites</span></span>
<span data-ttu-id="c5f2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f2d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f2d-110">Permission type</span></span>|<span data-ttu-id="c5f2d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5f2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f2d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5f2d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f2d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f2d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c5f2d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5f2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f2d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-115">Not supported.</span></span>|
|<span data-ttu-id="c5f2d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5f2d-116">Application</span></span>|<span data-ttu-id="c5f2d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f2d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f2d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5f2d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5f2d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5f2d-119">Optional query parameters</span></span>
<span data-ttu-id="c5f2d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5f2d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5f2d-121">Request headers</span></span>
|<span data-ttu-id="c5f2d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5f2d-122">Header</span></span>|<span data-ttu-id="c5f2d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f2d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f2d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5f2d-124">Authorization</span></span>|<span data-ttu-id="c5f2d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f2d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c5f2d-126">Accept</span></span>|<span data-ttu-id="c5f2d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f2d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f2d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5f2d-128">Request body</span></span>
<span data-ttu-id="c5f2d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f2d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5f2d-130">Response</span></span>
<span data-ttu-id="c5f2d-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-131">If successful, this method returns a `200 OK` response code and [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f2d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c5f2d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f2d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f2d-133">Request</span></span>
<span data-ttu-id="c5f2d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c5f2d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f2d-135">Response</span></span>
<span data-ttu-id="c5f2d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5f2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






