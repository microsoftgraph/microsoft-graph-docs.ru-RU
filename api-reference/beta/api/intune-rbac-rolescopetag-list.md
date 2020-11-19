---
title: Список roleScopeTags
description: Список свойств и связей объектов Ролескопетаг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b26d5d62744144066159fc147c82766090bc96ca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304478"
---
# <a name="list-rolescopetags"></a><span data-ttu-id="6a818-103">Список roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="6a818-103">List roleScopeTags</span></span>

<span data-ttu-id="6a818-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a818-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a818-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a818-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a818-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a818-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a818-107">Список свойств и связей объектов [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="6a818-107">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a818-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a818-108">Prerequisites</span></span>
<span data-ttu-id="6a818-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a818-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a818-111">Permission type</span></span>|<span data-ttu-id="6a818-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a818-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a818-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a818-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a818-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a818-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="6a818-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a818-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a818-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a818-116">Not supported.</span></span>|
|<span data-ttu-id="6a818-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a818-117">Application</span></span>|<span data-ttu-id="6a818-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a818-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a818-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a818-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="6a818-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a818-120">Request headers</span></span>
|<span data-ttu-id="6a818-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a818-121">Header</span></span>|<span data-ttu-id="6a818-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6a818-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a818-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a818-123">Authorization</span></span>|<span data-ttu-id="6a818-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a818-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a818-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a818-125">Accept</span></span>|<span data-ttu-id="6a818-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a818-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a818-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a818-127">Request body</span></span>
<span data-ttu-id="6a818-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a818-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a818-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a818-129">Response</span></span>
<span data-ttu-id="6a818-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a818-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a818-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6a818-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a818-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a818-132">Request</span></span>
<span data-ttu-id="6a818-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a818-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
```

### <a name="response"></a><span data-ttu-id="6a818-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a818-134">Response</span></span>
<span data-ttu-id="6a818-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




