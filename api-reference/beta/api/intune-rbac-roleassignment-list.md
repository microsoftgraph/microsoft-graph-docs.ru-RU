---
title: Список объектов roleAssignment
description: Список свойств и связей объектов roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39b7c379c7c5c764732e2c5d24f62f0b236bded9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420930"
---
# <a name="list-roleassignments"></a><span data-ttu-id="2197f-103">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2197f-103">List roleAssignments</span></span>

<span data-ttu-id="2197f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2197f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2197f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2197f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2197f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2197f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2197f-107">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2197f-107">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2197f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2197f-108">Prerequisites</span></span>
<span data-ttu-id="2197f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2197f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2197f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2197f-111">Permission type</span></span>|<span data-ttu-id="2197f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2197f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2197f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2197f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2197f-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2197f-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2197f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2197f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2197f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2197f-116">Not supported.</span></span>|
|<span data-ttu-id="2197f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2197f-117">Application</span></span>|<span data-ttu-id="2197f-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2197f-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2197f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2197f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="2197f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2197f-120">Request headers</span></span>
|<span data-ttu-id="2197f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2197f-121">Header</span></span>|<span data-ttu-id="2197f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2197f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2197f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2197f-123">Authorization</span></span>|<span data-ttu-id="2197f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2197f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2197f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2197f-125">Accept</span></span>|<span data-ttu-id="2197f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2197f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2197f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2197f-127">Request body</span></span>
<span data-ttu-id="2197f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2197f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2197f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2197f-129">Response</span></span>
<span data-ttu-id="2197f-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2197f-130">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2197f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2197f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2197f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2197f-132">Request</span></span>
<span data-ttu-id="2197f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2197f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="2197f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2197f-134">Response</span></span>
<span data-ttu-id="2197f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2197f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



