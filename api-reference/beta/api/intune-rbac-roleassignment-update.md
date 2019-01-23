---
title: Обновление объекта roleAssignment
description: Обновление свойств объекта roleAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dbb23619e6f44c9630d13808bb9263f21420d5b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414867"
---
# <a name="update-roleassignment"></a><span data-ttu-id="6234c-103">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="6234c-103">Update roleAssignment</span></span>

> <span data-ttu-id="6234c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6234c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6234c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6234c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6234c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6234c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6234c-107">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6234c-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6234c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6234c-108">Prerequisites</span></span>
<span data-ttu-id="6234c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6234c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6234c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6234c-111">Permission type</span></span>|<span data-ttu-id="6234c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6234c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6234c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6234c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6234c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6234c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6234c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6234c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6234c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6234c-116">Not supported.</span></span>|
|<span data-ttu-id="6234c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6234c-117">Application</span></span>|<span data-ttu-id="6234c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6234c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6234c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6234c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6234c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6234c-120">Request headers</span></span>
|<span data-ttu-id="6234c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6234c-121">Header</span></span>|<span data-ttu-id="6234c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6234c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6234c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6234c-123">Authorization</span></span>|<span data-ttu-id="6234c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6234c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6234c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6234c-125">Accept</span></span>|<span data-ttu-id="6234c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6234c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6234c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6234c-127">Request body</span></span>
<span data-ttu-id="6234c-128">В теле запроса добавьте представление объекта [roleAssignment](../resources/intune-rbac-roleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6234c-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="6234c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6234c-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="6234c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6234c-130">Property</span></span>|<span data-ttu-id="6234c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6234c-131">Type</span></span>|<span data-ttu-id="6234c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6234c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6234c-133">id</span><span class="sxs-lookup"><span data-stu-id="6234c-133">id</span></span>|<span data-ttu-id="6234c-134">String</span><span class="sxs-lookup"><span data-stu-id="6234c-134">String</span></span>|<span data-ttu-id="6234c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6234c-135">Key of the entity.</span></span> <span data-ttu-id="6234c-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="6234c-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="6234c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6234c-137">displayName</span></span>|<span data-ttu-id="6234c-138">String</span><span class="sxs-lookup"><span data-stu-id="6234c-138">String</span></span>|<span data-ttu-id="6234c-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="6234c-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="6234c-140">description</span><span class="sxs-lookup"><span data-stu-id="6234c-140">description</span></span>|<span data-ttu-id="6234c-141">String</span><span class="sxs-lookup"><span data-stu-id="6234c-141">String</span></span>|<span data-ttu-id="6234c-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="6234c-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="6234c-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="6234c-143">scopeMembers</span></span>|<span data-ttu-id="6234c-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6234c-144">String collection</span></span>|<span data-ttu-id="6234c-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="6234c-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6234c-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6234c-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="6234c-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="6234c-147">scopeType</span></span>|<span data-ttu-id="6234c-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="6234c-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="6234c-149">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="6234c-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="6234c-150">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="6234c-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="6234c-151">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="6234c-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="6234c-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="6234c-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="6234c-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="6234c-153">resourceScopes</span></span>|<span data-ttu-id="6234c-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6234c-154">String collection</span></span>|<span data-ttu-id="6234c-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="6234c-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6234c-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6234c-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="6234c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="6234c-157">Response</span></span>
<span data-ttu-id="6234c-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6234c-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6234c-159">Пример</span><span class="sxs-lookup"><span data-stu-id="6234c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6234c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="6234c-160">Request</span></span>
<span data-ttu-id="6234c-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6234c-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6234c-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6234c-162">Response</span></span>
<span data-ttu-id="6234c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6234c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




