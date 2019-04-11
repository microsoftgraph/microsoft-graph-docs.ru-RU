---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4df222bc2049fd7034e062eb2e6af8a86684cde6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778518"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="65080-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="65080-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="65080-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65080-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65080-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65080-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65080-106">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65080-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="65080-107">Prerequisites</span></span>
<span data-ttu-id="65080-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65080-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65080-110">Permission type</span></span>|<span data-ttu-id="65080-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65080-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65080-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65080-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65080-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65080-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="65080-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65080-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65080-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65080-115">Not supported.</span></span>|
|<span data-ttu-id="65080-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65080-116">Application</span></span>|<span data-ttu-id="65080-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65080-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65080-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65080-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="65080-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65080-119">Request headers</span></span>
|<span data-ttu-id="65080-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65080-120">Header</span></span>|<span data-ttu-id="65080-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65080-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65080-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65080-122">Authorization</span></span>|<span data-ttu-id="65080-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65080-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65080-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65080-124">Accept</span></span>|<span data-ttu-id="65080-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65080-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65080-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65080-126">Request body</span></span>
<span data-ttu-id="65080-127">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65080-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="65080-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="65080-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="65080-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="65080-129">Property</span></span>|<span data-ttu-id="65080-130">Тип</span><span class="sxs-lookup"><span data-stu-id="65080-130">Type</span></span>|<span data-ttu-id="65080-131">Описание</span><span class="sxs-lookup"><span data-stu-id="65080-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65080-132">id</span><span class="sxs-lookup"><span data-stu-id="65080-132">id</span></span>|<span data-ttu-id="65080-133">Строка</span><span class="sxs-lookup"><span data-stu-id="65080-133">String</span></span>|<span data-ttu-id="65080-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65080-134">Key of the entity.</span></span> <span data-ttu-id="65080-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="65080-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="65080-136">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="65080-137">displayName</span><span class="sxs-lookup"><span data-stu-id="65080-137">displayName</span></span>|<span data-ttu-id="65080-138">String</span><span class="sxs-lookup"><span data-stu-id="65080-138">String</span></span>|<span data-ttu-id="65080-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="65080-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="65080-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="65080-141">description</span><span class="sxs-lookup"><span data-stu-id="65080-141">description</span></span>|<span data-ttu-id="65080-142">String</span><span class="sxs-lookup"><span data-stu-id="65080-142">String</span></span>|<span data-ttu-id="65080-143">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="65080-143">Description of the Role Assignment.</span></span> <span data-ttu-id="65080-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="65080-145">Скопемемберс</span><span class="sxs-lookup"><span data-stu-id="65080-145">scopeMembers</span></span>|<span data-ttu-id="65080-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65080-146">String collection</span></span>|<span data-ttu-id="65080-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="65080-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="65080-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65080-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="65080-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="65080-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="65080-150">scopeType</span></span>|[<span data-ttu-id="65080-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="65080-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="65080-152">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="65080-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="65080-153">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="65080-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="65080-154">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="65080-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="65080-155">НаСледуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="65080-156">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="65080-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="65080-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="65080-157">resourceScopes</span></span>|<span data-ttu-id="65080-158">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="65080-158">String collection</span></span>|<span data-ttu-id="65080-159">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="65080-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="65080-160">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65080-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="65080-161">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="65080-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="65080-162">members</span><span class="sxs-lookup"><span data-stu-id="65080-162">members</span></span>|<span data-ttu-id="65080-163">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65080-163">String collection</span></span>|<span data-ttu-id="65080-164">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="65080-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="65080-165">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65080-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="65080-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="65080-166">Response</span></span>
<span data-ttu-id="65080-167">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65080-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65080-168">Пример</span><span class="sxs-lookup"><span data-stu-id="65080-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="65080-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="65080-169">Request</span></span>
<span data-ttu-id="65080-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65080-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="65080-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="65080-171">Response</span></span>
<span data-ttu-id="65080-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65080-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```





