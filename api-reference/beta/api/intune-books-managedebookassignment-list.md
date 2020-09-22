---
title: Перечисление объектов managedEBookAssignment
description: Список свойств и связей объектов managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 792a893c67c407314bf1bbfb6fdd1853fadf4e3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975530"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="e4e52-103">Перечисление объектов managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e4e52-103">List managedEBookAssignments</span></span>

<span data-ttu-id="e4e52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4e52-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4e52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4e52-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4e52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4e52-107">Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4e52-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4e52-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e4e52-108">Prerequisites</span></span>
<span data-ttu-id="e4e52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e52-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4e52-111">Permission type</span></span>|<span data-ttu-id="e4e52-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4e52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4e52-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4e52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4e52-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e52-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e4e52-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4e52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4e52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4e52-116">Not supported.</span></span>|
|<span data-ttu-id="e4e52-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4e52-117">Application</span></span>|<span data-ttu-id="e4e52-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e52-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4e52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4e52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e4e52-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4e52-120">Request headers</span></span>
|<span data-ttu-id="e4e52-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4e52-121">Header</span></span>|<span data-ttu-id="e4e52-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4e52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4e52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e52-123">Authorization</span></span>|<span data-ttu-id="e4e52-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4e52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4e52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4e52-125">Accept</span></span>|<span data-ttu-id="e4e52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4e52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e52-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4e52-127">Request body</span></span>
<span data-ttu-id="e4e52-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4e52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4e52-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4e52-129">Response</span></span>
<span data-ttu-id="e4e52-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4e52-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e52-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e4e52-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4e52-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4e52-132">Request</span></span>
<span data-ttu-id="e4e52-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4e52-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="e4e52-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4e52-134">Response</span></span>
<span data-ttu-id="e4e52-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4e52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 469

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "installIntent": "required"
    }
  ]
}
```






