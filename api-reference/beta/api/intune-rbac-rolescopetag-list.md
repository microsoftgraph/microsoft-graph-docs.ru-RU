---
title: Список roleScopeTags
description: Список свойств и связей объектов Ролескопетаг.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3705d14643ea05811d1b0bcb55b1818e068e93f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801574"
---
# <a name="list-rolescopetags"></a><span data-ttu-id="8cd9a-103">Список roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="8cd9a-103">List roleScopeTags</span></span>

> <span data-ttu-id="8cd9a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cd9a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cd9a-106">Список свойств и связей объектов [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="8cd9a-106">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cd9a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8cd9a-107">Prerequisites</span></span>
<span data-ttu-id="8cd9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cd9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd9a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd9a-110">Permission type</span></span>|<span data-ttu-id="8cd9a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cd9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cd9a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cd9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cd9a-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cd9a-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8cd9a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cd9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cd9a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-115">Not supported.</span></span>|
|<span data-ttu-id="8cd9a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8cd9a-116">Application</span></span>|<span data-ttu-id="8cd9a-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cd9a-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cd9a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cd9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="8cd9a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8cd9a-119">Request headers</span></span>
|<span data-ttu-id="8cd9a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cd9a-120">Header</span></span>|<span data-ttu-id="8cd9a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8cd9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cd9a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cd9a-122">Authorization</span></span>|<span data-ttu-id="8cd9a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cd9a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8cd9a-124">Accept</span></span>|<span data-ttu-id="8cd9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cd9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cd9a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cd9a-126">Request body</span></span>
<span data-ttu-id="8cd9a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cd9a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cd9a-128">Response</span></span>
<span data-ttu-id="8cd9a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-129">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cd9a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8cd9a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cd9a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cd9a-131">Request</span></span>
<span data-ttu-id="8cd9a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
```

### <a name="response"></a><span data-ttu-id="8cd9a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd9a-133">Response</span></span>
<span data-ttu-id="8cd9a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cd9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value",
      "isBuiltIn": true
    }
  ]
}
```




