---
title: Обновление объекта roleAssignment
description: Обновление свойств объекта roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06c71be971a4a3a37eed40568b3ec84d69d19b62
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512232"
---
# <a name="update-roleassignment"></a><span data-ttu-id="c1de6-103">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="c1de6-103">Update roleAssignment</span></span>

<span data-ttu-id="c1de6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1de6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1de6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1de6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1de6-106">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c1de6-106">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1de6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c1de6-107">Prerequisites</span></span>
<span data-ttu-id="c1de6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1de6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1de6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1de6-110">Permission type</span></span>|<span data-ttu-id="c1de6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1de6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1de6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1de6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1de6-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1de6-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c1de6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1de6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1de6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1de6-115">Not supported.</span></span>|
|<span data-ttu-id="c1de6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1de6-116">Application</span></span>|<span data-ttu-id="c1de6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1de6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1de6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1de6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1de6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1de6-119">Request headers</span></span>
|<span data-ttu-id="c1de6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1de6-120">Header</span></span>|<span data-ttu-id="c1de6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1de6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1de6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1de6-122">Authorization</span></span>|<span data-ttu-id="c1de6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1de6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1de6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c1de6-124">Accept</span></span>|<span data-ttu-id="c1de6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1de6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1de6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1de6-126">Request body</span></span>
<span data-ttu-id="c1de6-127">В теле запроса добавьте представление объекта [roleAssignment](../resources/intune-rbac-roleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1de6-127">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="c1de6-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c1de6-128">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="c1de6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1de6-129">Property</span></span>|<span data-ttu-id="c1de6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c1de6-130">Type</span></span>|<span data-ttu-id="c1de6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c1de6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1de6-132">id</span><span class="sxs-lookup"><span data-stu-id="c1de6-132">id</span></span>|<span data-ttu-id="c1de6-133">String</span><span class="sxs-lookup"><span data-stu-id="c1de6-133">String</span></span>|<span data-ttu-id="c1de6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1de6-134">Key of the entity.</span></span> <span data-ttu-id="c1de6-135">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="c1de6-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c1de6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c1de6-136">displayName</span></span>|<span data-ttu-id="c1de6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c1de6-137">String</span></span>|<span data-ttu-id="c1de6-138">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c1de6-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="c1de6-139">description</span><span class="sxs-lookup"><span data-stu-id="c1de6-139">description</span></span>|<span data-ttu-id="c1de6-140">String</span><span class="sxs-lookup"><span data-stu-id="c1de6-140">String</span></span>|<span data-ttu-id="c1de6-141">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c1de6-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="c1de6-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c1de6-142">resourceScopes</span></span>|<span data-ttu-id="c1de6-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1de6-143">String collection</span></span>|<span data-ttu-id="c1de6-144">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="c1de6-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c1de6-145">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1de6-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="c1de6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1de6-146">Response</span></span>
<span data-ttu-id="c1de6-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1de6-147">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1de6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c1de6-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1de6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1de6-149">Request</span></span>
<span data-ttu-id="c1de6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1de6-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="c1de6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1de6-151">Response</span></span>
<span data-ttu-id="c1de6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1de6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




