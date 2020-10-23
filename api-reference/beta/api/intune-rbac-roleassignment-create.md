---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 70b6ab750fb6e952a1454fed17f405a678280f9e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731493"
---
# <a name="create-roleassignment"></a><span data-ttu-id="af04c-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="af04c-103">Create roleAssignment</span></span>

<span data-ttu-id="af04c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af04c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af04c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af04c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af04c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af04c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af04c-107">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="af04c-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af04c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af04c-108">Prerequisites</span></span>
<span data-ttu-id="af04c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af04c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af04c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af04c-111">Permission type</span></span>|<span data-ttu-id="af04c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af04c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af04c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af04c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af04c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af04c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="af04c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af04c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af04c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af04c-116">Not supported.</span></span>|
|<span data-ttu-id="af04c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af04c-117">Application</span></span>|<span data-ttu-id="af04c-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af04c-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af04c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af04c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="af04c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af04c-120">Request headers</span></span>
|<span data-ttu-id="af04c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af04c-121">Header</span></span>|<span data-ttu-id="af04c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af04c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af04c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af04c-123">Authorization</span></span>|<span data-ttu-id="af04c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af04c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af04c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af04c-125">Accept</span></span>|<span data-ttu-id="af04c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af04c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af04c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af04c-127">Request body</span></span>
<span data-ttu-id="af04c-128">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af04c-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="af04c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="af04c-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="af04c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af04c-130">Property</span></span>|<span data-ttu-id="af04c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af04c-131">Type</span></span>|<span data-ttu-id="af04c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af04c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af04c-133">id</span><span class="sxs-lookup"><span data-stu-id="af04c-133">id</span></span>|<span data-ttu-id="af04c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="af04c-134">String</span></span>|<span data-ttu-id="af04c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af04c-135">Key of the entity.</span></span> <span data-ttu-id="af04c-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="af04c-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="af04c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="af04c-137">displayName</span></span>|<span data-ttu-id="af04c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="af04c-138">String</span></span>|<span data-ttu-id="af04c-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="af04c-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="af04c-140">description</span><span class="sxs-lookup"><span data-stu-id="af04c-140">description</span></span>|<span data-ttu-id="af04c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="af04c-141">String</span></span>|<span data-ttu-id="af04c-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="af04c-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="af04c-143">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="af04c-143">scopeMembers</span></span>|<span data-ttu-id="af04c-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af04c-144">String collection</span></span>|<span data-ttu-id="af04c-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="af04c-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="af04c-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af04c-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="af04c-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="af04c-147">scopeType</span></span>|<span data-ttu-id="af04c-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="af04c-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="af04c-149">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="af04c-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="af04c-150">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="af04c-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="af04c-151">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="af04c-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="af04c-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="af04c-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="af04c-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="af04c-153">resourceScopes</span></span>|<span data-ttu-id="af04c-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af04c-154">String collection</span></span>|<span data-ttu-id="af04c-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="af04c-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="af04c-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af04c-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="af04c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="af04c-157">Response</span></span>
<span data-ttu-id="af04c-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="af04c-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af04c-159">Пример</span><span class="sxs-lookup"><span data-stu-id="af04c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="af04c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="af04c-160">Request</span></span>
<span data-ttu-id="af04c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af04c-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af04c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="af04c-162">Response</span></span>
<span data-ttu-id="af04c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af04c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





