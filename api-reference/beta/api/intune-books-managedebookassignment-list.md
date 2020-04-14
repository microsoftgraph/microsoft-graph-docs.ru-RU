---
title: Перечисление объектов managedEBookAssignment
description: Список свойств и связей объектов managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5187607f9c2850d2632309931e7459b9a86947e5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392252"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="b7c86-103">Перечисление объектов managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="b7c86-103">List managedEBookAssignments</span></span>

<span data-ttu-id="b7c86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7c86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7c86-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7c86-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7c86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c86-107">Список свойств и связей объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b7c86-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7c86-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7c86-108">Prerequisites</span></span>
<span data-ttu-id="b7c86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c86-111">Permission type</span></span>|<span data-ttu-id="b7c86-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7c86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7c86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7c86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7c86-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7c86-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b7c86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7c86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7c86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c86-116">Not supported.</span></span>|
|<span data-ttu-id="b7c86-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b7c86-117">Application</span></span>|<span data-ttu-id="b7c86-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7c86-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7c86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7c86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b7c86-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b7c86-120">Request headers</span></span>
|<span data-ttu-id="b7c86-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7c86-121">Header</span></span>|<span data-ttu-id="b7c86-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b7c86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7c86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c86-123">Authorization</span></span>|<span data-ttu-id="b7c86-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7c86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7c86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7c86-125">Accept</span></span>|<span data-ttu-id="b7c86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7c86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c86-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7c86-127">Request body</span></span>
<span data-ttu-id="b7c86-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7c86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7c86-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7c86-129">Response</span></span>
<span data-ttu-id="b7c86-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7c86-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c86-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7c86-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7c86-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7c86-132">Request</span></span>
<span data-ttu-id="b7c86-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7c86-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="b7c86-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c86-134">Response</span></span>
<span data-ttu-id="b7c86-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7c86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```



