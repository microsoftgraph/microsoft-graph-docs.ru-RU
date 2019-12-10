---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78a950dac5d8901c03173bc6ff73a103349b9543
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940582"
---
# <a name="create-roleassignment"></a><span data-ttu-id="b4586-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b4586-103">Create roleAssignment</span></span>

> <span data-ttu-id="b4586-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4586-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4586-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4586-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4586-106">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b4586-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4586-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4586-107">Prerequisites</span></span>
<span data-ttu-id="b4586-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4586-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4586-110">Permission type</span></span>|<span data-ttu-id="b4586-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4586-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4586-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4586-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4586-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4586-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b4586-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4586-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4586-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4586-115">Not supported.</span></span>|
|<span data-ttu-id="b4586-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4586-116">Application</span></span>|<span data-ttu-id="b4586-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4586-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4586-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4586-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b4586-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4586-119">Request headers</span></span>
|<span data-ttu-id="b4586-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4586-120">Header</span></span>|<span data-ttu-id="b4586-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4586-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4586-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4586-122">Authorization</span></span>|<span data-ttu-id="b4586-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4586-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4586-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b4586-124">Accept</span></span>|<span data-ttu-id="b4586-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4586-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4586-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4586-126">Request body</span></span>
<span data-ttu-id="b4586-127">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4586-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="b4586-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="b4586-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="b4586-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4586-129">Property</span></span>|<span data-ttu-id="b4586-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4586-130">Type</span></span>|<span data-ttu-id="b4586-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4586-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4586-132">id</span><span class="sxs-lookup"><span data-stu-id="b4586-132">id</span></span>|<span data-ttu-id="b4586-133">String</span><span class="sxs-lookup"><span data-stu-id="b4586-133">String</span></span>|<span data-ttu-id="b4586-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4586-134">Key of the entity.</span></span> <span data-ttu-id="b4586-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="b4586-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b4586-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b4586-136">displayName</span></span>|<span data-ttu-id="b4586-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b4586-137">String</span></span>|<span data-ttu-id="b4586-138">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b4586-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b4586-139">description</span><span class="sxs-lookup"><span data-stu-id="b4586-139">description</span></span>|<span data-ttu-id="b4586-140">String</span><span class="sxs-lookup"><span data-stu-id="b4586-140">String</span></span>|<span data-ttu-id="b4586-141">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b4586-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b4586-142">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="b4586-142">scopeMembers</span></span>|<span data-ttu-id="b4586-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b4586-143">String collection</span></span>|<span data-ttu-id="b4586-144">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="b4586-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b4586-145">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4586-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="b4586-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="b4586-146">scopeType</span></span>|<span data-ttu-id="b4586-147">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="b4586-147">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="b4586-148">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b4586-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="b4586-149">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="b4586-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="b4586-150">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="b4586-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="b4586-151">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="b4586-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="b4586-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b4586-152">resourceScopes</span></span>|<span data-ttu-id="b4586-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b4586-153">String collection</span></span>|<span data-ttu-id="b4586-154">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="b4586-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b4586-155">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4586-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b4586-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4586-156">Response</span></span>
<span data-ttu-id="b4586-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4586-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4586-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b4586-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4586-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4586-159">Request</span></span>
<span data-ttu-id="b4586-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4586-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4586-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4586-161">Response</span></span>
<span data-ttu-id="b4586-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4586-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





