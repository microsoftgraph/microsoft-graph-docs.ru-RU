---
title: Перечисление объектов resourceOperation
description: Список свойств и связей объектов resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04c058ff0e88a925c52b1e3f66105068628200b2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685543"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="d5ef7-103">Перечисление объектов resourceOperation</span><span class="sxs-lookup"><span data-stu-id="d5ef7-103">List resourceOperations</span></span>

<span data-ttu-id="d5ef7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5ef7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5ef7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ef7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ef7-107">Список свойств и связей объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="d5ef7-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5ef7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5ef7-108">Prerequisites</span></span>
<span data-ttu-id="d5ef7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ef7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5ef7-111">Permission type</span></span>|<span data-ttu-id="d5ef7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5ef7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5ef7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5ef7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5ef7-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5ef7-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d5ef7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5ef7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5ef7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-116">Not supported.</span></span>|
|<span data-ttu-id="d5ef7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5ef7-117">Application</span></span>|<span data-ttu-id="d5ef7-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5ef7-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5ef7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5ef7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="d5ef7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5ef7-120">Request headers</span></span>
|<span data-ttu-id="d5ef7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5ef7-121">Header</span></span>|<span data-ttu-id="d5ef7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5ef7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5ef7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5ef7-123">Authorization</span></span>|<span data-ttu-id="d5ef7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5ef7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5ef7-125">Accept</span></span>|<span data-ttu-id="d5ef7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5ef7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5ef7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5ef7-127">Request body</span></span>
<span data-ttu-id="d5ef7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5ef7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5ef7-129">Response</span></span>
<span data-ttu-id="d5ef7-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5ef7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d5ef7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5ef7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5ef7-132">Request</span></span>
<span data-ttu-id="d5ef7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="d5ef7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5ef7-134">Response</span></span>
<span data-ttu-id="d5ef7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5ef7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```





