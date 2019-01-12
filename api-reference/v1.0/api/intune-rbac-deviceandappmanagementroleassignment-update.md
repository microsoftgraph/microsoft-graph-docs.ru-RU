---
title: Обновление объекта deviceAndAppManagementRoleAssignment
description: Обновление свойств объекта deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20f7299e80ae08aac8ce5c3d675bd411b6995dc4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963390"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="ff3c1-103">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff3c1-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="ff3c1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff3c1-105">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-105">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff3c1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff3c1-106">Prerequisites</span></span>
<span data-ttu-id="ff3c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff3c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff3c1-109">Permission type</span></span>|<span data-ttu-id="ff3c1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff3c1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff3c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff3c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff3c1-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff3c1-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ff3c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff3c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff3c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-114">Not supported.</span></span>|
|<span data-ttu-id="ff3c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff3c1-115">Application</span></span>|<span data-ttu-id="ff3c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff3c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff3c1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ff3c1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff3c1-118">Request headers</span></span>
|<span data-ttu-id="ff3c1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff3c1-119">Header</span></span>|<span data-ttu-id="ff3c1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ff3c1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff3c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff3c1-121">Authorization</span></span>|<span data-ttu-id="ff3c1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff3c1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff3c1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ff3c1-123">Accept</span></span>|<span data-ttu-id="ff3c1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff3c1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff3c1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff3c1-125">Request body</span></span>
<span data-ttu-id="ff3c1-126">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="ff3c1-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="ff3c1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff3c1-128">Property</span></span>|<span data-ttu-id="ff3c1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ff3c1-129">Type</span></span>|<span data-ttu-id="ff3c1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ff3c1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff3c1-131">id</span><span class="sxs-lookup"><span data-stu-id="ff3c1-131">id</span></span>|<span data-ttu-id="ff3c1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ff3c1-132">String</span></span>|<span data-ttu-id="ff3c1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-133">Key of the entity.</span></span> <span data-ttu-id="ff3c1-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="ff3c1-135">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ff3c1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ff3c1-136">displayName</span></span>|<span data-ttu-id="ff3c1-137">String</span><span class="sxs-lookup"><span data-stu-id="ff3c1-137">String</span></span>|<span data-ttu-id="ff3c1-138">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="ff3c1-139">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ff3c1-140">описание</span><span class="sxs-lookup"><span data-stu-id="ff3c1-140">description</span></span>|<span data-ttu-id="ff3c1-141">String</span><span class="sxs-lookup"><span data-stu-id="ff3c1-141">String</span></span>|<span data-ttu-id="ff3c1-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-142">Description of the Role Assignment.</span></span> <span data-ttu-id="ff3c1-143">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ff3c1-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ff3c1-144">resourceScopes</span></span>|<span data-ttu-id="ff3c1-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff3c1-145">String collection</span></span>|<span data-ttu-id="ff3c1-146">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ff3c1-147">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="ff3c1-148">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff3c1-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ff3c1-149">members</span><span class="sxs-lookup"><span data-stu-id="ff3c1-149">members</span></span>|<span data-ttu-id="ff3c1-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff3c1-150">String collection</span></span>|<span data-ttu-id="ff3c1-151">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="ff3c1-152">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="ff3c1-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff3c1-153">Response</span></span>
<span data-ttu-id="ff3c1-154">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-154">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff3c1-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ff3c1-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff3c1-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff3c1-156">Request</span></span>
<span data-ttu-id="ff3c1-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="ff3c1-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff3c1-158">Response</span></span>
<span data-ttu-id="ff3c1-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff3c1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



