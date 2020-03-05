---
title: Обновление объекта roleAssignment
description: Обновление свойств объекта roleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82bf64be5658606166bad9de48c1f44a2c68a73e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459697"
---
# <a name="update-roleassignment"></a><span data-ttu-id="4b633-103">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="4b633-103">Update roleAssignment</span></span>

<span data-ttu-id="4b633-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b633-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b633-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b633-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b633-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b633-107">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b633-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b633-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b633-108">Prerequisites</span></span>
<span data-ttu-id="4b633-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b633-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b633-111">Permission type</span></span>|<span data-ttu-id="4b633-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b633-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b633-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b633-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b633-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b633-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4b633-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b633-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b633-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b633-116">Not supported.</span></span>|
|<span data-ttu-id="4b633-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b633-117">Application</span></span>|<span data-ttu-id="4b633-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b633-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b633-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b633-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4b633-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b633-120">Request headers</span></span>
|<span data-ttu-id="4b633-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b633-121">Header</span></span>|<span data-ttu-id="4b633-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4b633-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b633-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b633-123">Authorization</span></span>|<span data-ttu-id="4b633-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b633-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b633-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b633-125">Accept</span></span>|<span data-ttu-id="4b633-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b633-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b633-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b633-127">Request body</span></span>
<span data-ttu-id="4b633-128">В теле запроса добавьте представление объекта [roleAssignment](../resources/intune-rbac-roleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b633-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="4b633-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b633-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="4b633-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b633-130">Property</span></span>|<span data-ttu-id="4b633-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b633-131">Type</span></span>|<span data-ttu-id="4b633-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b633-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b633-133">id</span><span class="sxs-lookup"><span data-stu-id="4b633-133">id</span></span>|<span data-ttu-id="4b633-134">String</span><span class="sxs-lookup"><span data-stu-id="4b633-134">String</span></span>|<span data-ttu-id="4b633-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b633-135">Key of the entity.</span></span> <span data-ttu-id="4b633-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4b633-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="4b633-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4b633-137">displayName</span></span>|<span data-ttu-id="4b633-138">Строка</span><span class="sxs-lookup"><span data-stu-id="4b633-138">String</span></span>|<span data-ttu-id="4b633-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4b633-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="4b633-140">description</span><span class="sxs-lookup"><span data-stu-id="4b633-140">description</span></span>|<span data-ttu-id="4b633-141">String</span><span class="sxs-lookup"><span data-stu-id="4b633-141">String</span></span>|<span data-ttu-id="4b633-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4b633-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="4b633-143">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="4b633-143">scopeMembers</span></span>|<span data-ttu-id="4b633-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b633-144">String collection</span></span>|<span data-ttu-id="4b633-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="4b633-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="4b633-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b633-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="4b633-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="4b633-147">scopeType</span></span>|<span data-ttu-id="4b633-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="4b633-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="4b633-149">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4b633-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="4b633-150">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="4b633-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="4b633-151">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="4b633-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="4b633-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="4b633-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="4b633-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="4b633-153">resourceScopes</span></span>|<span data-ttu-id="4b633-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b633-154">String collection</span></span>|<span data-ttu-id="4b633-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="4b633-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="4b633-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b633-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="4b633-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b633-157">Response</span></span>
<span data-ttu-id="4b633-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b633-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b633-159">Пример</span><span class="sxs-lookup"><span data-stu-id="4b633-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b633-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b633-160">Request</span></span>
<span data-ttu-id="4b633-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b633-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="4b633-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b633-162">Response</span></span>
<span data-ttu-id="4b633-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b633-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





