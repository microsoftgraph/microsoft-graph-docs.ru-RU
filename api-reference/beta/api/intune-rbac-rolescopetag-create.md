---
title: Создание Ролескопетаг
description: Создание нового объекта Ролескопетаг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 009a2f8f87c49495730b3f08be86b7238a119a97
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899433"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="92aa6-103">Создание Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="92aa6-103">Create roleScopeTag</span></span>

> <span data-ttu-id="92aa6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92aa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92aa6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92aa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92aa6-106">Создание нового объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="92aa6-106">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92aa6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92aa6-107">Prerequisites</span></span>
<span data-ttu-id="92aa6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92aa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92aa6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92aa6-110">Permission type</span></span>|<span data-ttu-id="92aa6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92aa6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92aa6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92aa6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92aa6-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92aa6-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="92aa6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92aa6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92aa6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92aa6-115">Not supported.</span></span>|
|<span data-ttu-id="92aa6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92aa6-116">Application</span></span>|<span data-ttu-id="92aa6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92aa6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92aa6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92aa6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="92aa6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92aa6-119">Request headers</span></span>
|<span data-ttu-id="92aa6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92aa6-120">Header</span></span>|<span data-ttu-id="92aa6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="92aa6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92aa6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92aa6-122">Authorization</span></span>|<span data-ttu-id="92aa6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92aa6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92aa6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92aa6-124">Accept</span></span>|<span data-ttu-id="92aa6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92aa6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92aa6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92aa6-126">Request body</span></span>
<span data-ttu-id="92aa6-127">В тексте запроса добавьте представление объекта Ролескопетаг в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92aa6-127">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="92aa6-128">В следующей таблице приведены свойства, необходимые при создании Ролескопетаг.</span><span class="sxs-lookup"><span data-stu-id="92aa6-128">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="92aa6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92aa6-129">Property</span></span>|<span data-ttu-id="92aa6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92aa6-130">Type</span></span>|<span data-ttu-id="92aa6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92aa6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92aa6-132">id</span><span class="sxs-lookup"><span data-stu-id="92aa6-132">id</span></span>|<span data-ttu-id="92aa6-133">String</span><span class="sxs-lookup"><span data-stu-id="92aa6-133">String</span></span>|<span data-ttu-id="92aa6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92aa6-134">Key of the entity.</span></span> <span data-ttu-id="92aa6-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="92aa6-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="92aa6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="92aa6-136">displayName</span></span>|<span data-ttu-id="92aa6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="92aa6-137">String</span></span>|<span data-ttu-id="92aa6-138">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="92aa6-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="92aa6-139">description</span><span class="sxs-lookup"><span data-stu-id="92aa6-139">description</span></span>|<span data-ttu-id="92aa6-140">String</span><span class="sxs-lookup"><span data-stu-id="92aa6-140">String</span></span>|<span data-ttu-id="92aa6-141">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="92aa6-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="92aa6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="92aa6-142">Response</span></span>
<span data-ttu-id="92aa6-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92aa6-143">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92aa6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="92aa6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="92aa6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="92aa6-145">Request</span></span>
<span data-ttu-id="92aa6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92aa6-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="92aa6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="92aa6-147">Response</span></span>
<span data-ttu-id="92aa6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92aa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




