---
title: Создание Ролескопетаг
description: Создание нового объекта Ролескопетаг.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 742e5b23c7296a1ad2a3e8654d2d844d76d48ecf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731486"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="5647a-103">Создание Ролескопетаг</span><span class="sxs-lookup"><span data-stu-id="5647a-103">Create roleScopeTag</span></span>

<span data-ttu-id="5647a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5647a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5647a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5647a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5647a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5647a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5647a-107">Создание нового объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="5647a-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5647a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5647a-108">Prerequisites</span></span>
<span data-ttu-id="5647a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5647a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5647a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5647a-111">Permission type</span></span>|<span data-ttu-id="5647a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5647a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5647a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5647a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5647a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5647a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5647a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5647a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5647a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5647a-116">Not supported.</span></span>|
|<span data-ttu-id="5647a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5647a-117">Application</span></span>|<span data-ttu-id="5647a-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5647a-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5647a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5647a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="5647a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5647a-120">Request headers</span></span>
|<span data-ttu-id="5647a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5647a-121">Header</span></span>|<span data-ttu-id="5647a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5647a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5647a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5647a-123">Authorization</span></span>|<span data-ttu-id="5647a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5647a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5647a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5647a-125">Accept</span></span>|<span data-ttu-id="5647a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5647a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5647a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5647a-127">Request body</span></span>
<span data-ttu-id="5647a-128">В тексте запроса добавьте представление объекта Ролескопетаг в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5647a-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="5647a-129">В следующей таблице приведены свойства, необходимые при создании Ролескопетаг.</span><span class="sxs-lookup"><span data-stu-id="5647a-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="5647a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5647a-130">Property</span></span>|<span data-ttu-id="5647a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5647a-131">Type</span></span>|<span data-ttu-id="5647a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5647a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5647a-133">id</span><span class="sxs-lookup"><span data-stu-id="5647a-133">id</span></span>|<span data-ttu-id="5647a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5647a-134">String</span></span>|<span data-ttu-id="5647a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5647a-135">Key of the entity.</span></span> <span data-ttu-id="5647a-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5647a-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5647a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5647a-137">displayName</span></span>|<span data-ttu-id="5647a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5647a-138">String</span></span>|<span data-ttu-id="5647a-139">Отображаемое или понятное имя тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="5647a-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="5647a-140">description</span><span class="sxs-lookup"><span data-stu-id="5647a-140">description</span></span>|<span data-ttu-id="5647a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5647a-141">String</span></span>|<span data-ttu-id="5647a-142">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="5647a-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="5647a-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5647a-143">isBuiltIn</span></span>|<span data-ttu-id="5647a-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5647a-144">Boolean</span></span>|<span data-ttu-id="5647a-145">Описание тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="5647a-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="5647a-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="5647a-146">Response</span></span>
<span data-ttu-id="5647a-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5647a-147">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5647a-148">Пример</span><span class="sxs-lookup"><span data-stu-id="5647a-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="5647a-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5647a-149">Request</span></span>
<span data-ttu-id="5647a-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5647a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5647a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5647a-151">Response</span></span>
<span data-ttu-id="5647a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5647a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





