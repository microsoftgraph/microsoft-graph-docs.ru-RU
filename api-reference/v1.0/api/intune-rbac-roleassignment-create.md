---
title: Создание объекта roleAssignment
description: Создание объекта roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 837c69f2bf23c662c86769b308eae205767ca453
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361821"
---
# <a name="create-roleassignment"></a><span data-ttu-id="d49ba-103">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d49ba-103">Create roleAssignment</span></span>

> <span data-ttu-id="d49ba-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d49ba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d49ba-105">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d49ba-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d49ba-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d49ba-106">Prerequisites</span></span>
<span data-ttu-id="d49ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d49ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d49ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d49ba-109">Permission type</span></span>|<span data-ttu-id="d49ba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d49ba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d49ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d49ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d49ba-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d49ba-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d49ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d49ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d49ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d49ba-114">Not supported.</span></span>|
|<span data-ttu-id="d49ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d49ba-115">Application</span></span>|<span data-ttu-id="d49ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d49ba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d49ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d49ba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d49ba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d49ba-118">Request headers</span></span>
|<span data-ttu-id="d49ba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d49ba-119">Header</span></span>|<span data-ttu-id="d49ba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d49ba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d49ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d49ba-121">Authorization</span></span>|<span data-ttu-id="d49ba-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d49ba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d49ba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d49ba-123">Accept</span></span>|<span data-ttu-id="d49ba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d49ba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d49ba-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d49ba-125">Request body</span></span>
<span data-ttu-id="d49ba-126">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d49ba-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="d49ba-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d49ba-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="d49ba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d49ba-128">Property</span></span>|<span data-ttu-id="d49ba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d49ba-129">Type</span></span>|<span data-ttu-id="d49ba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d49ba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d49ba-131">id</span><span class="sxs-lookup"><span data-stu-id="d49ba-131">id</span></span>|<span data-ttu-id="d49ba-132">String</span><span class="sxs-lookup"><span data-stu-id="d49ba-132">String</span></span>|<span data-ttu-id="d49ba-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d49ba-133">Key of the entity.</span></span> <span data-ttu-id="d49ba-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="d49ba-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d49ba-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d49ba-135">displayName</span></span>|<span data-ttu-id="d49ba-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d49ba-136">String</span></span>|<span data-ttu-id="d49ba-137">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d49ba-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d49ba-138">description</span><span class="sxs-lookup"><span data-stu-id="d49ba-138">description</span></span>|<span data-ttu-id="d49ba-139">String</span><span class="sxs-lookup"><span data-stu-id="d49ba-139">String</span></span>|<span data-ttu-id="d49ba-140">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d49ba-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d49ba-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d49ba-141">resourceScopes</span></span>|<span data-ttu-id="d49ba-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d49ba-142">String collection</span></span>|<span data-ttu-id="d49ba-143">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="d49ba-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d49ba-144">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d49ba-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="d49ba-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d49ba-145">Response</span></span>
<span data-ttu-id="d49ba-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d49ba-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d49ba-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d49ba-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d49ba-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d49ba-148">Request</span></span>
<span data-ttu-id="d49ba-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d49ba-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d49ba-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d49ba-150">Response</span></span>
<span data-ttu-id="d49ba-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d49ba-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




