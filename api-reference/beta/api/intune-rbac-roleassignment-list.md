---
title: Список объектов roleAssignment
description: Список свойств и связей объектов roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e9d03f661edb87bbf342a53ec9be82592f31d79
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148332"
---
# <a name="list-roleassignments"></a><span data-ttu-id="c9373-103">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="c9373-103">List roleAssignments</span></span>

<span data-ttu-id="c9373-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9373-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9373-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9373-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9373-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9373-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9373-107">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9373-107">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9373-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9373-108">Prerequisites</span></span>
<span data-ttu-id="c9373-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9373-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9373-111">Permission type</span></span>|<span data-ttu-id="c9373-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9373-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9373-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9373-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9373-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9373-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c9373-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9373-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9373-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9373-116">Not supported.</span></span>|
|<span data-ttu-id="c9373-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c9373-117">Application</span></span>|<span data-ttu-id="c9373-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9373-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9373-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9373-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c9373-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9373-120">Request headers</span></span>
|<span data-ttu-id="c9373-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9373-121">Header</span></span>|<span data-ttu-id="c9373-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9373-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9373-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9373-123">Authorization</span></span>|<span data-ttu-id="c9373-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9373-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9373-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9373-125">Accept</span></span>|<span data-ttu-id="c9373-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9373-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9373-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9373-127">Request body</span></span>
<span data-ttu-id="c9373-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9373-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9373-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9373-129">Response</span></span>
<span data-ttu-id="c9373-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9373-130">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9373-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c9373-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9373-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9373-132">Request</span></span>
<span data-ttu-id="c9373-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9373-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="c9373-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9373-134">Response</span></span>
<span data-ttu-id="c9373-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9373-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```




