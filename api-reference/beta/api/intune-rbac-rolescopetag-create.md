---
title: Создание roleScopeTag
description: Создайте новый объект roleScopeTag.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7d02eb907ee0fbedde3240906277601eca8601e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156669"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="beb2e-103">Создание roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="beb2e-103">Create roleScopeTag</span></span>

<span data-ttu-id="beb2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="beb2e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beb2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="beb2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beb2e-107">Создайте новый [объект roleScopeTag.](../resources/intune-rbac-rolescopetag.md)</span><span class="sxs-lookup"><span data-stu-id="beb2e-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="beb2e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="beb2e-108">Prerequisites</span></span>
<span data-ttu-id="beb2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beb2e-111">Permission type</span></span>|<span data-ttu-id="beb2e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beb2e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beb2e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beb2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="beb2e-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb2e-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="beb2e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beb2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beb2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beb2e-116">Not supported.</span></span>|
|<span data-ttu-id="beb2e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="beb2e-117">Application</span></span>|<span data-ttu-id="beb2e-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb2e-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="beb2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beb2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="beb2e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="beb2e-120">Request headers</span></span>
|<span data-ttu-id="beb2e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="beb2e-121">Header</span></span>|<span data-ttu-id="beb2e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="beb2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beb2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="beb2e-123">Authorization</span></span>|<span data-ttu-id="beb2e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beb2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beb2e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="beb2e-125">Accept</span></span>|<span data-ttu-id="beb2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="beb2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beb2e-127">Request body</span></span>
<span data-ttu-id="beb2e-128">В теле запроса поставляем представление JSON для объекта roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="beb2e-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="beb2e-129">В следующей таблице показаны свойства, необходимые при создании roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="beb2e-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="beb2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="beb2e-130">Property</span></span>|<span data-ttu-id="beb2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="beb2e-131">Type</span></span>|<span data-ttu-id="beb2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="beb2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb2e-133">id</span><span class="sxs-lookup"><span data-stu-id="beb2e-133">id</span></span>|<span data-ttu-id="beb2e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="beb2e-134">String</span></span>|<span data-ttu-id="beb2e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="beb2e-135">Key of the entity.</span></span> <span data-ttu-id="beb2e-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="beb2e-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="beb2e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="beb2e-137">displayName</span></span>|<span data-ttu-id="beb2e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="beb2e-138">String</span></span>|<span data-ttu-id="beb2e-139">Отображение или дружеское имя тега Область ролей.</span><span class="sxs-lookup"><span data-stu-id="beb2e-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="beb2e-140">description</span><span class="sxs-lookup"><span data-stu-id="beb2e-140">description</span></span>|<span data-ttu-id="beb2e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="beb2e-141">String</span></span>|<span data-ttu-id="beb2e-142">Описание тега Область ролей.</span><span class="sxs-lookup"><span data-stu-id="beb2e-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="beb2e-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="beb2e-143">isBuiltIn</span></span>|<span data-ttu-id="beb2e-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb2e-144">Boolean</span></span>|<span data-ttu-id="beb2e-145">Описание тега Область ролей.</span><span class="sxs-lookup"><span data-stu-id="beb2e-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="beb2e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb2e-146">Response</span></span>
<span data-ttu-id="beb2e-147">В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [roleScopeTag](../resources/intune-rbac-rolescopetag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="beb2e-147">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb2e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="beb2e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb2e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="beb2e-149">Request</span></span>
<span data-ttu-id="beb2e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beb2e-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="beb2e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="beb2e-151">Response</span></span>
<span data-ttu-id="beb2e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="beb2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




