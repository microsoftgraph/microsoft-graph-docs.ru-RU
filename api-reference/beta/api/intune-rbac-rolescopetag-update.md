---
title: Обновление Ролескопетаг
description: Обновление свойств объекта Ролескопетаг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1dd417be2450f7cc956f6e6c4c7c39f9f748be2d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955128"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="26a57-103">Обновление Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="26a57-103">Update roleScopeTag</span></span>

> <span data-ttu-id="26a57-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a57-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26a57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a57-106">Обновление свойств объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="26a57-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26a57-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26a57-107">Prerequisites</span></span>
<span data-ttu-id="26a57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a57-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26a57-110">Permission type</span></span>|<span data-ttu-id="26a57-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26a57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26a57-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26a57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26a57-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a57-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="26a57-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26a57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26a57-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a57-115">Not supported.</span></span>|
|<span data-ttu-id="26a57-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26a57-116">Application</span></span>|<span data-ttu-id="26a57-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a57-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26a57-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26a57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="26a57-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26a57-119">Request headers</span></span>
|<span data-ttu-id="26a57-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26a57-120">Header</span></span>|<span data-ttu-id="26a57-121">Значение</span><span class="sxs-lookup"><span data-stu-id="26a57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26a57-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26a57-122">Authorization</span></span>|<span data-ttu-id="26a57-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26a57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26a57-124">Accept</span><span class="sxs-lookup"><span data-stu-id="26a57-124">Accept</span></span>|<span data-ttu-id="26a57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26a57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26a57-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26a57-126">Request body</span></span>
<span data-ttu-id="26a57-127">В тексте запроса добавьте представление объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a57-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="26a57-128">В следующей таблице приведены свойства, необходимые при создании [ролескопетаг](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="26a57-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="26a57-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="26a57-129">Property</span></span>|<span data-ttu-id="26a57-130">Тип</span><span class="sxs-lookup"><span data-stu-id="26a57-130">Type</span></span>|<span data-ttu-id="26a57-131">Описание</span><span class="sxs-lookup"><span data-stu-id="26a57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a57-132">id</span><span class="sxs-lookup"><span data-stu-id="26a57-132">id</span></span>|<span data-ttu-id="26a57-133">String</span><span class="sxs-lookup"><span data-stu-id="26a57-133">String</span></span>|<span data-ttu-id="26a57-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26a57-134">Key of the entity.</span></span> <span data-ttu-id="26a57-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="26a57-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="26a57-136">displayName</span><span class="sxs-lookup"><span data-stu-id="26a57-136">displayName</span></span>|<span data-ttu-id="26a57-137">Строка</span><span class="sxs-lookup"><span data-stu-id="26a57-137">String</span></span>|<span data-ttu-id="26a57-138">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="26a57-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="26a57-139">description</span><span class="sxs-lookup"><span data-stu-id="26a57-139">description</span></span>|<span data-ttu-id="26a57-140">String</span><span class="sxs-lookup"><span data-stu-id="26a57-140">String</span></span>|<span data-ttu-id="26a57-141">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="26a57-141">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="26a57-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="26a57-142">isBuiltIn</span></span>|<span data-ttu-id="26a57-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="26a57-143">Boolean</span></span>|<span data-ttu-id="26a57-144">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="26a57-144">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="26a57-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="26a57-145">Response</span></span>
<span data-ttu-id="26a57-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26a57-146">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a57-147">Пример</span><span class="sxs-lookup"><span data-stu-id="26a57-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="26a57-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="26a57-148">Request</span></span>
<span data-ttu-id="26a57-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26a57-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26a57-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a57-150">Response</span></span>
<span data-ttu-id="26a57-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26a57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





