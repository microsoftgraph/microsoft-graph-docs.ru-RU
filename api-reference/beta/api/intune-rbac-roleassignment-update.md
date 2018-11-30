---
title: Обновление объекта roleAssignment
description: Обновление свойств объекта roleAssignment.
ms.openlocfilehash: 64ec4aa3c885ce2c9de475faef1e00fd14f2576d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076690"
---
# <a name="update-roleassignment"></a><span data-ttu-id="067d0-103">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="067d0-103">Update roleAssignment</span></span>

> <span data-ttu-id="067d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="067d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="067d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="067d0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="067d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="067d0-107">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="067d0-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="067d0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="067d0-108">Prerequisites</span></span>
<span data-ttu-id="067d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="067d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="067d0-111">Permission type</span></span>|<span data-ttu-id="067d0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="067d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="067d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="067d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="067d0-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="067d0-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="067d0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="067d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="067d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067d0-116">Not supported.</span></span>|
|<span data-ttu-id="067d0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="067d0-117">Application</span></span>|<span data-ttu-id="067d0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="067d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="067d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="067d0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="067d0-120">Request headers</span></span>
|<span data-ttu-id="067d0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="067d0-121">Header</span></span>|<span data-ttu-id="067d0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="067d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="067d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="067d0-123">Authorization</span></span>|<span data-ttu-id="067d0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="067d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="067d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="067d0-125">Accept</span></span>|<span data-ttu-id="067d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="067d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="067d0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="067d0-127">Request body</span></span>
<span data-ttu-id="067d0-128">В теле запроса добавьте представление объекта [roleAssignment](../resources/intune-rbac-roleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="067d0-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="067d0-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="067d0-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="067d0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="067d0-130">Property</span></span>|<span data-ttu-id="067d0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="067d0-131">Type</span></span>|<span data-ttu-id="067d0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="067d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="067d0-133">id</span><span class="sxs-lookup"><span data-stu-id="067d0-133">id</span></span>|<span data-ttu-id="067d0-134">String</span><span class="sxs-lookup"><span data-stu-id="067d0-134">String</span></span>|<span data-ttu-id="067d0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="067d0-135">Key of the entity.</span></span> <span data-ttu-id="067d0-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="067d0-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="067d0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="067d0-137">displayName</span></span>|<span data-ttu-id="067d0-138">String</span><span class="sxs-lookup"><span data-stu-id="067d0-138">String</span></span>|<span data-ttu-id="067d0-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="067d0-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="067d0-140">описание</span><span class="sxs-lookup"><span data-stu-id="067d0-140">description</span></span>|<span data-ttu-id="067d0-141">String</span><span class="sxs-lookup"><span data-stu-id="067d0-141">String</span></span>|<span data-ttu-id="067d0-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="067d0-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="067d0-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="067d0-143">scopeMembers</span></span>|<span data-ttu-id="067d0-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="067d0-144">String collection</span></span>|<span data-ttu-id="067d0-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="067d0-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="067d0-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="067d0-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="067d0-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="067d0-147">scopeType</span></span>|<span data-ttu-id="067d0-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="067d0-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="067d0-149">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="067d0-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="067d0-150">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="067d0-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="067d0-151">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="067d0-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="067d0-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="067d0-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="067d0-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="067d0-153">resourceScopes</span></span>|<span data-ttu-id="067d0-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="067d0-154">String collection</span></span>|<span data-ttu-id="067d0-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="067d0-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="067d0-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="067d0-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="067d0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="067d0-157">Response</span></span>
<span data-ttu-id="067d0-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="067d0-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="067d0-159">Пример</span><span class="sxs-lookup"><span data-stu-id="067d0-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="067d0-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="067d0-160">Request</span></span>
<span data-ttu-id="067d0-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="067d0-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 224

{
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

### <a name="response"></a><span data-ttu-id="067d0-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="067d0-162">Response</span></span>
<span data-ttu-id="067d0-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="067d0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





