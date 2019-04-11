---
title: Список объектов roleAssignment
description: Список свойств и связей объектов roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b986699f73174fd224d62a4aeec75d53d30f86c6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778208"
---
# <a name="list-roleassignments"></a><span data-ttu-id="891e2-103">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="891e2-103">List roleAssignments</span></span>

> <span data-ttu-id="891e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="891e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="891e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="891e2-106">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="891e2-106">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="891e2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="891e2-107">Prerequisites</span></span>
<span data-ttu-id="891e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="891e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="891e2-110">Permission type</span></span>|<span data-ttu-id="891e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="891e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="891e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="891e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="891e2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="891e2-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="891e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="891e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="891e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891e2-115">Not supported.</span></span>|
|<span data-ttu-id="891e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="891e2-116">Application</span></span>|<span data-ttu-id="891e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="891e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="891e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="891e2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="891e2-119">Request headers</span></span>
|<span data-ttu-id="891e2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="891e2-120">Header</span></span>|<span data-ttu-id="891e2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="891e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="891e2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="891e2-122">Authorization</span></span>|<span data-ttu-id="891e2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="891e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="891e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="891e2-124">Accept</span></span>|<span data-ttu-id="891e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="891e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="891e2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="891e2-126">Request body</span></span>
<span data-ttu-id="891e2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="891e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="891e2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="891e2-128">Response</span></span>
<span data-ttu-id="891e2-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="891e2-129">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="891e2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="891e2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="891e2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="891e2-131">Request</span></span>
<span data-ttu-id="891e2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="891e2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="891e2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="891e2-133">Response</span></span>
<span data-ttu-id="891e2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="891e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





