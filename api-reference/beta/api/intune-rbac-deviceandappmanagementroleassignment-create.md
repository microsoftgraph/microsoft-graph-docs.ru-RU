---
title: Создание объекта deviceAndAppManagementRoleAssignment
description: Создание объекта deviceAndAppManagementRoleAssignment.
author: tfitzmac
ms.openlocfilehash: 4ed81fdc58a2675be6d5f0b991507914d5c92e89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323991"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="ea9af-103">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea9af-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="ea9af-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea9af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea9af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea9af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea9af-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea9af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea9af-107">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea9af-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ea9af-108">Prerequisites</span></span>
<span data-ttu-id="ea9af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea9af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea9af-111">Permission type</span></span>|<span data-ttu-id="ea9af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea9af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea9af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea9af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea9af-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea9af-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ea9af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea9af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea9af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea9af-116">Not supported.</span></span>|
|<span data-ttu-id="ea9af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea9af-117">Application</span></span>|<span data-ttu-id="ea9af-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea9af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea9af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea9af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ea9af-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea9af-120">Request headers</span></span>
|<span data-ttu-id="ea9af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea9af-121">Header</span></span>|<span data-ttu-id="ea9af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea9af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea9af-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea9af-123">Authorization</span></span>|<span data-ttu-id="ea9af-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ea9af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea9af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea9af-125">Accept</span></span>|<span data-ttu-id="ea9af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea9af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea9af-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea9af-127">Request body</span></span>
<span data-ttu-id="ea9af-128">В теле запроса добавьте представление объекта deviceAndAppManagementRoleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea9af-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="ea9af-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ea9af-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="ea9af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea9af-130">Property</span></span>|<span data-ttu-id="ea9af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea9af-131">Type</span></span>|<span data-ttu-id="ea9af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea9af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea9af-133">id</span><span class="sxs-lookup"><span data-stu-id="ea9af-133">id</span></span>|<span data-ttu-id="ea9af-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ea9af-134">String</span></span>|<span data-ttu-id="ea9af-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea9af-135">Key of the entity.</span></span> <span data-ttu-id="ea9af-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ea9af-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="ea9af-137">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ea9af-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ea9af-138">displayName</span></span>|<span data-ttu-id="ea9af-139">String</span><span class="sxs-lookup"><span data-stu-id="ea9af-139">String</span></span>|<span data-ttu-id="ea9af-140">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ea9af-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="ea9af-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ea9af-142">описание</span><span class="sxs-lookup"><span data-stu-id="ea9af-142">description</span></span>|<span data-ttu-id="ea9af-143">String</span><span class="sxs-lookup"><span data-stu-id="ea9af-143">String</span></span>|<span data-ttu-id="ea9af-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ea9af-144">Description of the Role Assignment.</span></span> <span data-ttu-id="ea9af-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ea9af-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="ea9af-146">scopeMembers</span></span>|<span data-ttu-id="ea9af-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea9af-147">String collection</span></span>|<span data-ttu-id="ea9af-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ea9af-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ea9af-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea9af-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="ea9af-150">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ea9af-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="ea9af-151">scopeType</span></span>|<span data-ttu-id="ea9af-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="ea9af-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="ea9af-153">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="ea9af-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="ea9af-154">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="ea9af-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="ea9af-155">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="ea9af-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="ea9af-156">Наследуется от [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="ea9af-157">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="ea9af-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="ea9af-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ea9af-158">resourceScopes</span></span>|<span data-ttu-id="ea9af-159">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea9af-159">String collection</span></span>|<span data-ttu-id="ea9af-160">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ea9af-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ea9af-161">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea9af-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="ea9af-162">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea9af-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="ea9af-163">members</span><span class="sxs-lookup"><span data-stu-id="ea9af-163">members</span></span>|<span data-ttu-id="ea9af-164">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea9af-164">String collection</span></span>|<span data-ttu-id="ea9af-165">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="ea9af-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="ea9af-166">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea9af-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="ea9af-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea9af-167">Response</span></span>
<span data-ttu-id="ea9af-168">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea9af-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea9af-169">Пример</span><span class="sxs-lookup"><span data-stu-id="ea9af-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea9af-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea9af-170">Request</span></span>
<span data-ttu-id="ea9af-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea9af-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea9af-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea9af-172">Response</span></span>
<span data-ttu-id="ea9af-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ea9af-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





