---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6019357dcea7e020022eb5def2d449c9a5be47cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456590"
---
# <a name="create-roleassignment"></a><span data-ttu-id="263aa-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="263aa-103">Create roleAssignment</span></span>

<span data-ttu-id="263aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="263aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="263aa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="263aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="263aa-106">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="263aa-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="263aa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="263aa-107">Prerequisites</span></span>
<span data-ttu-id="263aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="263aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="263aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="263aa-110">Permission type</span></span>|<span data-ttu-id="263aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="263aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="263aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="263aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="263aa-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="263aa-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="263aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="263aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="263aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="263aa-115">Not supported.</span></span>|
|<span data-ttu-id="263aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="263aa-116">Application</span></span>|<span data-ttu-id="263aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="263aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="263aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="263aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="263aa-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="263aa-119">Request headers</span></span>
|<span data-ttu-id="263aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="263aa-120">Header</span></span>|<span data-ttu-id="263aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="263aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="263aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="263aa-122">Authorization</span></span>|<span data-ttu-id="263aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="263aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="263aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="263aa-124">Accept</span></span>|<span data-ttu-id="263aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="263aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="263aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="263aa-126">Request body</span></span>
<span data-ttu-id="263aa-127">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="263aa-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="263aa-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="263aa-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="263aa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="263aa-129">Property</span></span>|<span data-ttu-id="263aa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="263aa-130">Type</span></span>|<span data-ttu-id="263aa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="263aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="263aa-132">id</span><span class="sxs-lookup"><span data-stu-id="263aa-132">id</span></span>|<span data-ttu-id="263aa-133">String</span><span class="sxs-lookup"><span data-stu-id="263aa-133">String</span></span>|<span data-ttu-id="263aa-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="263aa-134">Key of the entity.</span></span> <span data-ttu-id="263aa-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="263aa-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="263aa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="263aa-136">displayName</span></span>|<span data-ttu-id="263aa-137">Строка</span><span class="sxs-lookup"><span data-stu-id="263aa-137">String</span></span>|<span data-ttu-id="263aa-138">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="263aa-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="263aa-139">description</span><span class="sxs-lookup"><span data-stu-id="263aa-139">description</span></span>|<span data-ttu-id="263aa-140">String</span><span class="sxs-lookup"><span data-stu-id="263aa-140">String</span></span>|<span data-ttu-id="263aa-141">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="263aa-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="263aa-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="263aa-142">resourceScopes</span></span>|<span data-ttu-id="263aa-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="263aa-143">String collection</span></span>|<span data-ttu-id="263aa-144">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="263aa-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="263aa-145">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="263aa-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="263aa-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="263aa-146">Response</span></span>
<span data-ttu-id="263aa-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="263aa-147">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263aa-148">Пример</span><span class="sxs-lookup"><span data-stu-id="263aa-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="263aa-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="263aa-149">Request</span></span>
<span data-ttu-id="263aa-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="263aa-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="263aa-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="263aa-151">Response</span></span>
<span data-ttu-id="263aa-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="263aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```






