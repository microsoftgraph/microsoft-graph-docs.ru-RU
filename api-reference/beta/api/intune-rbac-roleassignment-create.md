---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a8c889e401664fb0fea66030ff3bcabd0631503
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399915"
---
# <a name="create-roleassignment"></a><span data-ttu-id="77721-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="77721-103">Create roleAssignment</span></span>

> <span data-ttu-id="77721-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77721-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77721-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77721-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77721-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77721-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77721-107">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="77721-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77721-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77721-108">Prerequisites</span></span>
<span data-ttu-id="77721-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77721-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77721-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77721-111">Permission type</span></span>|<span data-ttu-id="77721-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77721-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77721-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77721-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77721-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77721-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="77721-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77721-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77721-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77721-116">Not supported.</span></span>|
|<span data-ttu-id="77721-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77721-117">Application</span></span>|<span data-ttu-id="77721-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77721-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77721-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77721-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="77721-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77721-120">Request headers</span></span>
|<span data-ttu-id="77721-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77721-121">Header</span></span>|<span data-ttu-id="77721-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77721-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77721-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77721-123">Authorization</span></span>|<span data-ttu-id="77721-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77721-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77721-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77721-125">Accept</span></span>|<span data-ttu-id="77721-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77721-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77721-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77721-127">Request body</span></span>
<span data-ttu-id="77721-128">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77721-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="77721-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="77721-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="77721-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77721-130">Property</span></span>|<span data-ttu-id="77721-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77721-131">Type</span></span>|<span data-ttu-id="77721-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77721-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77721-133">id</span><span class="sxs-lookup"><span data-stu-id="77721-133">id</span></span>|<span data-ttu-id="77721-134">String</span><span class="sxs-lookup"><span data-stu-id="77721-134">String</span></span>|<span data-ttu-id="77721-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77721-135">Key of the entity.</span></span> <span data-ttu-id="77721-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="77721-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="77721-137">displayName</span><span class="sxs-lookup"><span data-stu-id="77721-137">displayName</span></span>|<span data-ttu-id="77721-138">String</span><span class="sxs-lookup"><span data-stu-id="77721-138">String</span></span>|<span data-ttu-id="77721-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="77721-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="77721-140">description</span><span class="sxs-lookup"><span data-stu-id="77721-140">description</span></span>|<span data-ttu-id="77721-141">String</span><span class="sxs-lookup"><span data-stu-id="77721-141">String</span></span>|<span data-ttu-id="77721-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="77721-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="77721-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="77721-143">scopeMembers</span></span>|<span data-ttu-id="77721-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77721-144">String collection</span></span>|<span data-ttu-id="77721-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="77721-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="77721-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77721-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="77721-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="77721-147">scopeType</span></span>|<span data-ttu-id="77721-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="77721-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="77721-149">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="77721-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="77721-150">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="77721-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="77721-151">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="77721-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="77721-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="77721-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="77721-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="77721-153">resourceScopes</span></span>|<span data-ttu-id="77721-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77721-154">String collection</span></span>|<span data-ttu-id="77721-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="77721-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="77721-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77721-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="77721-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="77721-157">Response</span></span>
<span data-ttu-id="77721-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77721-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77721-159">Пример</span><span class="sxs-lookup"><span data-stu-id="77721-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="77721-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="77721-160">Request</span></span>
<span data-ttu-id="77721-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77721-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="77721-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="77721-162">Response</span></span>
<span data-ttu-id="77721-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="77721-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```




