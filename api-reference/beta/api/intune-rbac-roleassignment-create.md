---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: becb8ec776092e966bf4af24fc2c32dcad10a6a9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421019"
---
# <a name="create-roleassignment"></a><span data-ttu-id="740cb-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="740cb-103">Create roleAssignment</span></span>

<span data-ttu-id="740cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="740cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="740cb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="740cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="740cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="740cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="740cb-107">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="740cb-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="740cb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="740cb-108">Prerequisites</span></span>
<span data-ttu-id="740cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="740cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="740cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="740cb-111">Permission type</span></span>|<span data-ttu-id="740cb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="740cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="740cb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="740cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="740cb-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="740cb-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="740cb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="740cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="740cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="740cb-116">Not supported.</span></span>|
|<span data-ttu-id="740cb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="740cb-117">Application</span></span>|<span data-ttu-id="740cb-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="740cb-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="740cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="740cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="740cb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="740cb-120">Request headers</span></span>
|<span data-ttu-id="740cb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="740cb-121">Header</span></span>|<span data-ttu-id="740cb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="740cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="740cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="740cb-123">Authorization</span></span>|<span data-ttu-id="740cb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="740cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="740cb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="740cb-125">Accept</span></span>|<span data-ttu-id="740cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="740cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="740cb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="740cb-127">Request body</span></span>
<span data-ttu-id="740cb-128">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="740cb-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="740cb-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="740cb-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="740cb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="740cb-130">Property</span></span>|<span data-ttu-id="740cb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="740cb-131">Type</span></span>|<span data-ttu-id="740cb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="740cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="740cb-133">id</span><span class="sxs-lookup"><span data-stu-id="740cb-133">id</span></span>|<span data-ttu-id="740cb-134">String</span><span class="sxs-lookup"><span data-stu-id="740cb-134">String</span></span>|<span data-ttu-id="740cb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="740cb-135">Key of the entity.</span></span> <span data-ttu-id="740cb-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="740cb-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="740cb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="740cb-137">displayName</span></span>|<span data-ttu-id="740cb-138">Строка</span><span class="sxs-lookup"><span data-stu-id="740cb-138">String</span></span>|<span data-ttu-id="740cb-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="740cb-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="740cb-140">description</span><span class="sxs-lookup"><span data-stu-id="740cb-140">description</span></span>|<span data-ttu-id="740cb-141">String</span><span class="sxs-lookup"><span data-stu-id="740cb-141">String</span></span>|<span data-ttu-id="740cb-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="740cb-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="740cb-143">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="740cb-143">scopeMembers</span></span>|<span data-ttu-id="740cb-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="740cb-144">String collection</span></span>|<span data-ttu-id="740cb-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="740cb-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="740cb-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="740cb-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="740cb-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="740cb-147">scopeType</span></span>|<span data-ttu-id="740cb-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="740cb-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="740cb-149">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="740cb-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="740cb-150">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="740cb-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="740cb-151">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="740cb-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="740cb-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="740cb-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="740cb-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="740cb-153">resourceScopes</span></span>|<span data-ttu-id="740cb-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="740cb-154">String collection</span></span>|<span data-ttu-id="740cb-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="740cb-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="740cb-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="740cb-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="740cb-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="740cb-157">Response</span></span>
<span data-ttu-id="740cb-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="740cb-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="740cb-159">Пример</span><span class="sxs-lookup"><span data-stu-id="740cb-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="740cb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="740cb-160">Request</span></span>
<span data-ttu-id="740cb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="740cb-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="740cb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="740cb-162">Response</span></span>
<span data-ttu-id="740cb-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="740cb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



