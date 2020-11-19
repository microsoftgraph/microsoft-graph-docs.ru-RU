---
title: действие Жетролескопетагсбид
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f68df95361826868767d3e85012624a5b6caef0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304590"
---
# <a name="getrolescopetagsbyid-action"></a><span data-ttu-id="dc9e2-103">действие Жетролескопетагсбид</span><span class="sxs-lookup"><span data-stu-id="dc9e2-103">getRoleScopeTagsById action</span></span>

<span data-ttu-id="dc9e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc9e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc9e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc9e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc9e2-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc9e2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dc9e2-108">Prerequisites</span></span>
<span data-ttu-id="dc9e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc9e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc9e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc9e2-111">Permission type</span></span>|<span data-ttu-id="dc9e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc9e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc9e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc9e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc9e2-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc9e2-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="dc9e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc9e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc9e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-116">Not supported.</span></span>|
|<span data-ttu-id="dc9e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc9e2-117">Application</span></span>|<span data-ttu-id="dc9e2-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc9e2-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc9e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc9e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a><span data-ttu-id="dc9e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc9e2-120">Request headers</span></span>
|<span data-ttu-id="dc9e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc9e2-121">Header</span></span>|<span data-ttu-id="dc9e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc9e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc9e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc9e2-123">Authorization</span></span>|<span data-ttu-id="dc9e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc9e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc9e2-125">Accept</span></span>|<span data-ttu-id="dc9e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc9e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc9e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc9e2-127">Request body</span></span>
<span data-ttu-id="dc9e2-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dc9e2-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dc9e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc9e2-130">Property</span></span>|<span data-ttu-id="dc9e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc9e2-131">Type</span></span>|<span data-ttu-id="dc9e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc9e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc9e2-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dc9e2-133">roleScopeTagIds</span></span>|<span data-ttu-id="dc9e2-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dc9e2-134">String collection</span></span>|<span data-ttu-id="dc9e2-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dc9e2-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dc9e2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc9e2-136">Response</span></span>
<span data-ttu-id="dc9e2-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-137">If successful, this action returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc9e2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dc9e2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc9e2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc9e2-139">Request</span></span>
<span data-ttu-id="dc9e2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/getRoleScopeTagsById

Content-type: application/json
Content-length: 65

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dc9e2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9e2-141">Response</span></span>
<span data-ttu-id="dc9e2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc9e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




