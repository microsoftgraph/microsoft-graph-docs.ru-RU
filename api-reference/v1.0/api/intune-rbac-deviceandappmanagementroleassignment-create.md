---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: edd6878f8bebbff66114814067e8d76056f5baf4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362031"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="26377-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="26377-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="26377-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26377-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26377-105">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26377-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26377-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="26377-106">Prerequisites</span></span>
<span data-ttu-id="26377-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26377-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26377-109">Permission type</span></span>|<span data-ttu-id="26377-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26377-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26377-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26377-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26377-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26377-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="26377-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26377-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26377-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26377-114">Not supported.</span></span>|
|<span data-ttu-id="26377-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26377-115">Application</span></span>|<span data-ttu-id="26377-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26377-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26377-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26377-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="26377-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26377-118">Request headers</span></span>
|<span data-ttu-id="26377-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26377-119">Header</span></span>|<span data-ttu-id="26377-120">Значение</span><span class="sxs-lookup"><span data-stu-id="26377-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26377-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26377-121">Authorization</span></span>|<span data-ttu-id="26377-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26377-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26377-123">Accept</span><span class="sxs-lookup"><span data-stu-id="26377-123">Accept</span></span>|<span data-ttu-id="26377-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26377-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26377-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26377-125">Request body</span></span>
<span data-ttu-id="26377-126">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26377-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="26377-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="26377-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="26377-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="26377-128">Property</span></span>|<span data-ttu-id="26377-129">Тип</span><span class="sxs-lookup"><span data-stu-id="26377-129">Type</span></span>|<span data-ttu-id="26377-130">Описание</span><span class="sxs-lookup"><span data-stu-id="26377-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26377-131">id</span><span class="sxs-lookup"><span data-stu-id="26377-131">id</span></span>|<span data-ttu-id="26377-132">String</span><span class="sxs-lookup"><span data-stu-id="26377-132">String</span></span>|<span data-ttu-id="26377-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26377-133">Key of the entity.</span></span> <span data-ttu-id="26377-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="26377-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="26377-135">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26377-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="26377-136">displayName</span><span class="sxs-lookup"><span data-stu-id="26377-136">displayName</span></span>|<span data-ttu-id="26377-137">Строка</span><span class="sxs-lookup"><span data-stu-id="26377-137">String</span></span>|<span data-ttu-id="26377-138">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="26377-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="26377-139">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26377-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="26377-140">description</span><span class="sxs-lookup"><span data-stu-id="26377-140">description</span></span>|<span data-ttu-id="26377-141">String</span><span class="sxs-lookup"><span data-stu-id="26377-141">String</span></span>|<span data-ttu-id="26377-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="26377-142">Description of the Role Assignment.</span></span> <span data-ttu-id="26377-143">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26377-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="26377-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="26377-144">resourceScopes</span></span>|<span data-ttu-id="26377-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="26377-145">String collection</span></span>|<span data-ttu-id="26377-146">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="26377-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="26377-147">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="26377-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="26377-148">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="26377-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="26377-149">members</span><span class="sxs-lookup"><span data-stu-id="26377-149">members</span></span>|<span data-ttu-id="26377-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26377-150">String collection</span></span>|<span data-ttu-id="26377-151">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="26377-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="26377-152">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="26377-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="26377-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="26377-153">Response</span></span>
<span data-ttu-id="26377-154">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26377-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26377-155">Пример</span><span class="sxs-lookup"><span data-stu-id="26377-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="26377-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="26377-156">Request</span></span>
<span data-ttu-id="26377-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26377-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26377-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="26377-158">Response</span></span>
<span data-ttu-id="26377-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26377-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




