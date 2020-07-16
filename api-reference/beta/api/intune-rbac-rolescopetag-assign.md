---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b49619c3340c4e920d5a5e4cb30ad1978f5cd422
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791688"
---
# <a name="assign-action"></a><span data-ttu-id="d5ebe-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="d5ebe-103">assign action</span></span>

<span data-ttu-id="d5ebe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5ebe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5ebe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ebe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ebe-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5ebe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5ebe-108">Prerequisites</span></span>
<span data-ttu-id="d5ebe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ebe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5ebe-111">Permission type</span></span>|<span data-ttu-id="d5ebe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5ebe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5ebe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5ebe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5ebe-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ebe-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d5ebe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5ebe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5ebe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-116">Not supported.</span></span>|
|<span data-ttu-id="d5ebe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5ebe-117">Application</span></span>|<span data-ttu-id="d5ebe-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ebe-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5ebe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5ebe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/{roleScopeTagId}/assign
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d5ebe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5ebe-120">Request headers</span></span>
|<span data-ttu-id="d5ebe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5ebe-121">Header</span></span>|<span data-ttu-id="d5ebe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5ebe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5ebe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5ebe-123">Authorization</span></span>|<span data-ttu-id="d5ebe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5ebe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5ebe-125">Accept</span></span>|<span data-ttu-id="d5ebe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5ebe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5ebe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5ebe-127">Request body</span></span>
<span data-ttu-id="d5ebe-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d5ebe-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d5ebe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5ebe-130">Property</span></span>|<span data-ttu-id="d5ebe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d5ebe-131">Type</span></span>|<span data-ttu-id="d5ebe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d5ebe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5ebe-133">assignments</span><span class="sxs-lookup"><span data-stu-id="d5ebe-133">assignments</span></span>|<span data-ttu-id="d5ebe-134">Коллекция [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d5ebe-134">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="d5ebe-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d5ebe-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d5ebe-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5ebe-136">Response</span></span>
<span data-ttu-id="d5ebe-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-137">If successful, this action returns a `200 OK` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5ebe-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d5ebe-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5ebe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5ebe-139">Request</span></span>
<span data-ttu-id="d5ebe-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}/assign

Content-type: application/json
Content-length: 437

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d5ebe-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5ebe-141">Response</span></span>
<span data-ttu-id="d5ebe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5ebe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 431

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



