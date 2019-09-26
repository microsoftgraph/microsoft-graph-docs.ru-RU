---
title: Обновление Ролескопетаг
description: Обновление свойств объекта Ролескопетаг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3abe206624e1d24d515059a86e3272c591643ec8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194938"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="8f380-103">Обновление Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="8f380-103">Update roleScopeTag</span></span>

> <span data-ttu-id="8f380-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f380-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f380-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f380-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f380-106">Обновление свойств объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="8f380-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f380-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f380-107">Prerequisites</span></span>
<span data-ttu-id="8f380-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f380-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f380-110">Permission type</span></span>|<span data-ttu-id="8f380-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f380-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f380-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f380-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f380-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f380-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8f380-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f380-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f380-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f380-115">Not supported.</span></span>|
|<span data-ttu-id="8f380-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f380-116">Application</span></span>|<span data-ttu-id="8f380-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f380-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f380-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f380-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="8f380-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f380-119">Request headers</span></span>
|<span data-ttu-id="8f380-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f380-120">Header</span></span>|<span data-ttu-id="8f380-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8f380-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f380-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f380-122">Authorization</span></span>|<span data-ttu-id="8f380-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f380-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f380-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8f380-124">Accept</span></span>|<span data-ttu-id="8f380-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f380-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f380-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f380-126">Request body</span></span>
<span data-ttu-id="8f380-127">В тексте запроса добавьте представление объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f380-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="8f380-128">В следующей таблице приведены свойства, необходимые при создании [ролескопетаг](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="8f380-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="8f380-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f380-129">Property</span></span>|<span data-ttu-id="8f380-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8f380-130">Type</span></span>|<span data-ttu-id="8f380-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8f380-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f380-132">id</span><span class="sxs-lookup"><span data-stu-id="8f380-132">id</span></span>|<span data-ttu-id="8f380-133">String</span><span class="sxs-lookup"><span data-stu-id="8f380-133">String</span></span>|<span data-ttu-id="8f380-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f380-134">Key of the entity.</span></span> <span data-ttu-id="8f380-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="8f380-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="8f380-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8f380-136">displayName</span></span>|<span data-ttu-id="8f380-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8f380-137">String</span></span>|<span data-ttu-id="8f380-138">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="8f380-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="8f380-139">description</span><span class="sxs-lookup"><span data-stu-id="8f380-139">description</span></span>|<span data-ttu-id="8f380-140">String</span><span class="sxs-lookup"><span data-stu-id="8f380-140">String</span></span>|<span data-ttu-id="8f380-141">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="8f380-141">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="8f380-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8f380-142">isBuiltIn</span></span>|<span data-ttu-id="8f380-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f380-143">Boolean</span></span>|<span data-ttu-id="8f380-144">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="8f380-144">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="8f380-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f380-145">Response</span></span>
<span data-ttu-id="8f380-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f380-146">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f380-147">Пример</span><span class="sxs-lookup"><span data-stu-id="8f380-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f380-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f380-148">Request</span></span>
<span data-ttu-id="8f380-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f380-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f380-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f380-150">Response</span></span>
<span data-ttu-id="8f380-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f380-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




