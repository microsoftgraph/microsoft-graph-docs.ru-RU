---
title: Перечисление объектов managedEBookAssignment
description: Список свойств и связей объектов managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ae058914393ce885965827ad20ef7dd9c7b2e02
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244971"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="611cc-103">Перечисление объектов managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="611cc-103">List managedEBookAssignments</span></span>

<span data-ttu-id="611cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="611cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="611cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="611cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="611cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="611cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="611cc-107">Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="611cc-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="611cc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="611cc-108">Prerequisites</span></span>
<span data-ttu-id="611cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="611cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="611cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="611cc-111">Permission type</span></span>|<span data-ttu-id="611cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="611cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="611cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="611cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="611cc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="611cc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="611cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="611cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="611cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="611cc-116">Not supported.</span></span>|
|<span data-ttu-id="611cc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="611cc-117">Application</span></span>|<span data-ttu-id="611cc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="611cc-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="611cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="611cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="611cc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="611cc-120">Request headers</span></span>
|<span data-ttu-id="611cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="611cc-121">Header</span></span>|<span data-ttu-id="611cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="611cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="611cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="611cc-123">Authorization</span></span>|<span data-ttu-id="611cc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="611cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="611cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="611cc-125">Accept</span></span>|<span data-ttu-id="611cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="611cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="611cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="611cc-127">Request body</span></span>
<span data-ttu-id="611cc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="611cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="611cc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="611cc-129">Response</span></span>
<span data-ttu-id="611cc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="611cc-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="611cc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="611cc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="611cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="611cc-132">Request</span></span>
<span data-ttu-id="611cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="611cc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="611cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="611cc-134">Response</span></span>
<span data-ttu-id="611cc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="611cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




