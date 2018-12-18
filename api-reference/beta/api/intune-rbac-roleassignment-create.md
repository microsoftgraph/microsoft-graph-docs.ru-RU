---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
author: tfitzmac
ms.openlocfilehash: bf255b0d2c077cbba2e34e81d9730e51c4f5d813
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359747"
---
# <a name="create-roleassignment"></a><span data-ttu-id="c53e5-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="c53e5-103">Create roleAssignment</span></span>

> <span data-ttu-id="c53e5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c53e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c53e5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c53e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c53e5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c53e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c53e5-107">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c53e5-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c53e5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c53e5-108">Prerequisites</span></span>
<span data-ttu-id="c53e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c53e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c53e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c53e5-111">Permission type</span></span>|<span data-ttu-id="c53e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c53e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c53e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c53e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c53e5-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c53e5-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c53e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c53e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c53e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c53e5-116">Not supported.</span></span>|
|<span data-ttu-id="c53e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c53e5-117">Application</span></span>|<span data-ttu-id="c53e5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c53e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c53e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c53e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c53e5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c53e5-120">Request headers</span></span>
|<span data-ttu-id="c53e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c53e5-121">Header</span></span>|<span data-ttu-id="c53e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c53e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c53e5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c53e5-123">Authorization</span></span>|<span data-ttu-id="c53e5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c53e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c53e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c53e5-125">Accept</span></span>|<span data-ttu-id="c53e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c53e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c53e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c53e5-127">Request body</span></span>
<span data-ttu-id="c53e5-128">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c53e5-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="c53e5-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="c53e5-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="c53e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c53e5-130">Property</span></span>|<span data-ttu-id="c53e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c53e5-131">Type</span></span>|<span data-ttu-id="c53e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c53e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c53e5-133">id</span><span class="sxs-lookup"><span data-stu-id="c53e5-133">id</span></span>|<span data-ttu-id="c53e5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c53e5-134">String</span></span>|<span data-ttu-id="c53e5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c53e5-135">Key of the entity.</span></span> <span data-ttu-id="c53e5-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="c53e5-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c53e5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c53e5-137">displayName</span></span>|<span data-ttu-id="c53e5-138">String</span><span class="sxs-lookup"><span data-stu-id="c53e5-138">String</span></span>|<span data-ttu-id="c53e5-139">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c53e5-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="c53e5-140">описание</span><span class="sxs-lookup"><span data-stu-id="c53e5-140">description</span></span>|<span data-ttu-id="c53e5-141">String</span><span class="sxs-lookup"><span data-stu-id="c53e5-141">String</span></span>|<span data-ttu-id="c53e5-142">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c53e5-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="c53e5-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="c53e5-143">scopeMembers</span></span>|<span data-ttu-id="c53e5-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c53e5-144">String collection</span></span>|<span data-ttu-id="c53e5-145">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="c53e5-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c53e5-146">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c53e5-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="c53e5-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="c53e5-147">scopeType</span></span>|<span data-ttu-id="c53e5-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="c53e5-148">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="c53e5-149">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="c53e5-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="c53e5-150">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="c53e5-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="c53e5-151">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="c53e5-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="c53e5-152">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="c53e5-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="c53e5-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c53e5-153">resourceScopes</span></span>|<span data-ttu-id="c53e5-154">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c53e5-154">String collection</span></span>|<span data-ttu-id="c53e5-155">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="c53e5-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c53e5-156">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c53e5-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="c53e5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c53e5-157">Response</span></span>
<span data-ttu-id="c53e5-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c53e5-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c53e5-159">Пример</span><span class="sxs-lookup"><span data-stu-id="c53e5-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="c53e5-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c53e5-160">Request</span></span>
<span data-ttu-id="c53e5-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c53e5-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c53e5-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="c53e5-162">Response</span></span>
<span data-ttu-id="c53e5-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c53e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





