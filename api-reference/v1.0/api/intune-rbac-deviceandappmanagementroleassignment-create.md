---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
ms.openlocfilehash: bdfb17c1f6e1bc9ea75c6ee72e0277efd5295035
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026609"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="5030b-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5030b-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="5030b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5030b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5030b-105">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5030b-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5030b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5030b-106">Prerequisites</span></span>
<span data-ttu-id="5030b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5030b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5030b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5030b-109">Permission type</span></span>|<span data-ttu-id="5030b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5030b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5030b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5030b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5030b-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5030b-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5030b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5030b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5030b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5030b-114">Not supported.</span></span>|
|<span data-ttu-id="5030b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5030b-115">Application</span></span>|<span data-ttu-id="5030b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5030b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5030b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5030b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="5030b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5030b-118">Request headers</span></span>
|<span data-ttu-id="5030b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5030b-119">Header</span></span>|<span data-ttu-id="5030b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5030b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5030b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5030b-121">Authorization</span></span>|<span data-ttu-id="5030b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5030b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5030b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5030b-123">Accept</span></span>|<span data-ttu-id="5030b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5030b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5030b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5030b-125">Request body</span></span>
<span data-ttu-id="5030b-126">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5030b-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="5030b-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="5030b-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="5030b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5030b-128">Property</span></span>|<span data-ttu-id="5030b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5030b-129">Type</span></span>|<span data-ttu-id="5030b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5030b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5030b-131">id</span><span class="sxs-lookup"><span data-stu-id="5030b-131">id</span></span>|<span data-ttu-id="5030b-132">String</span><span class="sxs-lookup"><span data-stu-id="5030b-132">String</span></span>|<span data-ttu-id="5030b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5030b-133">Key of the entity.</span></span> <span data-ttu-id="5030b-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5030b-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="5030b-135">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5030b-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5030b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5030b-136">displayName</span></span>|<span data-ttu-id="5030b-137">String</span><span class="sxs-lookup"><span data-stu-id="5030b-137">String</span></span>|<span data-ttu-id="5030b-138">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5030b-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="5030b-139">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5030b-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5030b-140">описание</span><span class="sxs-lookup"><span data-stu-id="5030b-140">description</span></span>|<span data-ttu-id="5030b-141">String</span><span class="sxs-lookup"><span data-stu-id="5030b-141">String</span></span>|<span data-ttu-id="5030b-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5030b-142">Description of the Role Assignment.</span></span> <span data-ttu-id="5030b-143">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5030b-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5030b-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="5030b-144">resourceScopes</span></span>|<span data-ttu-id="5030b-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5030b-145">String collection</span></span>|<span data-ttu-id="5030b-146">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="5030b-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5030b-147">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5030b-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5030b-148">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5030b-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5030b-149">members</span><span class="sxs-lookup"><span data-stu-id="5030b-149">members</span></span>|<span data-ttu-id="5030b-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5030b-150">String collection</span></span>|<span data-ttu-id="5030b-151">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="5030b-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="5030b-152">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5030b-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="5030b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5030b-153">Response</span></span>
<span data-ttu-id="5030b-154">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5030b-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5030b-155">Пример</span><span class="sxs-lookup"><span data-stu-id="5030b-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="5030b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="5030b-156">Request</span></span>
<span data-ttu-id="5030b-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5030b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5030b-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="5030b-158">Response</span></span>
<span data-ttu-id="5030b-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5030b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



