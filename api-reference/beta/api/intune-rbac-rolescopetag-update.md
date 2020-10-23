---
title: Обновление Ролескопетаг
description: Обновление свойств объекта Ролескопетаг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b06b776aa51f160071a482b3619a93ce7a0edda1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724644"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="506af-103">Обновление Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="506af-103">Update roleScopeTag</span></span>

<span data-ttu-id="506af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="506af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="506af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="506af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="506af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="506af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="506af-107">Обновление свойств объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="506af-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="506af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="506af-108">Prerequisites</span></span>
<span data-ttu-id="506af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="506af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="506af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="506af-111">Permission type</span></span>|<span data-ttu-id="506af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="506af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="506af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="506af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="506af-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="506af-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="506af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="506af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="506af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="506af-116">Not supported.</span></span>|
|<span data-ttu-id="506af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="506af-117">Application</span></span>|<span data-ttu-id="506af-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="506af-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="506af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="506af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="506af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="506af-120">Request headers</span></span>
|<span data-ttu-id="506af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="506af-121">Header</span></span>|<span data-ttu-id="506af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="506af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="506af-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="506af-123">Authorization</span></span>|<span data-ttu-id="506af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="506af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="506af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="506af-125">Accept</span></span>|<span data-ttu-id="506af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="506af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="506af-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="506af-127">Request body</span></span>
<span data-ttu-id="506af-128">В тексте запроса добавьте представление объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="506af-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="506af-129">В следующей таблице приведены свойства, необходимые при создании [ролескопетаг](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="506af-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="506af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="506af-130">Property</span></span>|<span data-ttu-id="506af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="506af-131">Type</span></span>|<span data-ttu-id="506af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="506af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="506af-133">id</span><span class="sxs-lookup"><span data-stu-id="506af-133">id</span></span>|<span data-ttu-id="506af-134">Строка</span><span class="sxs-lookup"><span data-stu-id="506af-134">String</span></span>|<span data-ttu-id="506af-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="506af-135">Key of the entity.</span></span> <span data-ttu-id="506af-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="506af-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="506af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="506af-137">displayName</span></span>|<span data-ttu-id="506af-138">Строка</span><span class="sxs-lookup"><span data-stu-id="506af-138">String</span></span>|<span data-ttu-id="506af-139">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="506af-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="506af-140">description</span><span class="sxs-lookup"><span data-stu-id="506af-140">description</span></span>|<span data-ttu-id="506af-141">Строка</span><span class="sxs-lookup"><span data-stu-id="506af-141">String</span></span>|<span data-ttu-id="506af-142">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="506af-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="506af-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="506af-143">isBuiltIn</span></span>|<span data-ttu-id="506af-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="506af-144">Boolean</span></span>|<span data-ttu-id="506af-145">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="506af-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="506af-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="506af-146">Response</span></span>
<span data-ttu-id="506af-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="506af-147">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="506af-148">Пример</span><span class="sxs-lookup"><span data-stu-id="506af-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="506af-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="506af-149">Request</span></span>
<span data-ttu-id="506af-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="506af-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="506af-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="506af-151">Response</span></span>
<span data-ttu-id="506af-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="506af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





