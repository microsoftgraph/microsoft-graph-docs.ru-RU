---
title: Обновление Ролескопетаг
description: Обновление свойств объекта Ролескопетаг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09126c70c36ee6d73554fd1ec10799ad47c7eeb8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459500"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="c5bf8-103">Обновление Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="c5bf8-103">Update roleScopeTag</span></span>

<span data-ttu-id="c5bf8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c5bf8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5bf8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5bf8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5bf8-107">Обновление свойств объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="c5bf8-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5bf8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5bf8-108">Prerequisites</span></span>
<span data-ttu-id="c5bf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5bf8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bf8-111">Permission type</span></span>|<span data-ttu-id="c5bf8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5bf8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5bf8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5bf8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5bf8-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bf8-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c5bf8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5bf8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5bf8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-116">Not supported.</span></span>|
|<span data-ttu-id="c5bf8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5bf8-117">Application</span></span>|<span data-ttu-id="c5bf8-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bf8-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5bf8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5bf8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="c5bf8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5bf8-120">Request headers</span></span>
|<span data-ttu-id="c5bf8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5bf8-121">Header</span></span>|<span data-ttu-id="c5bf8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5bf8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5bf8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5bf8-123">Authorization</span></span>|<span data-ttu-id="c5bf8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5bf8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5bf8-125">Accept</span></span>|<span data-ttu-id="c5bf8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5bf8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5bf8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5bf8-127">Request body</span></span>
<span data-ttu-id="c5bf8-128">В тексте запроса добавьте представление объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="c5bf8-129">В следующей таблице приведены свойства, необходимые при создании [ролескопетаг](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="c5bf8-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="c5bf8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5bf8-130">Property</span></span>|<span data-ttu-id="c5bf8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5bf8-131">Type</span></span>|<span data-ttu-id="c5bf8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5bf8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5bf8-133">id</span><span class="sxs-lookup"><span data-stu-id="c5bf8-133">id</span></span>|<span data-ttu-id="c5bf8-134">String</span><span class="sxs-lookup"><span data-stu-id="c5bf8-134">String</span></span>|<span data-ttu-id="c5bf8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-135">Key of the entity.</span></span> <span data-ttu-id="c5bf8-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c5bf8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c5bf8-137">displayName</span></span>|<span data-ttu-id="c5bf8-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c5bf8-138">String</span></span>|<span data-ttu-id="c5bf8-139">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="c5bf8-140">description</span><span class="sxs-lookup"><span data-stu-id="c5bf8-140">description</span></span>|<span data-ttu-id="c5bf8-141">String</span><span class="sxs-lookup"><span data-stu-id="c5bf8-141">String</span></span>|<span data-ttu-id="c5bf8-142">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="c5bf8-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c5bf8-143">isBuiltIn</span></span>|<span data-ttu-id="c5bf8-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5bf8-144">Boolean</span></span>|<span data-ttu-id="c5bf8-145">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="c5bf8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5bf8-146">Response</span></span>
<span data-ttu-id="c5bf8-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-147">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5bf8-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c5bf8-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5bf8-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5bf8-149">Request</span></span>
<span data-ttu-id="c5bf8-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="c5bf8-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5bf8-151">Response</span></span>
<span data-ttu-id="c5bf8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5bf8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```





