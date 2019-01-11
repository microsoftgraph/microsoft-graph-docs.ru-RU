---
title: Обновление объекта roleAssignment
description: Обновление свойств объекта roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: edcfa7d06cbe4348835109c2adc3a48d9f24fe7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816214"
---
# <a name="update-roleassignment"></a><span data-ttu-id="b52ad-103">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b52ad-103">Update roleAssignment</span></span>

> <span data-ttu-id="b52ad-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b52ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b52ad-105">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b52ad-105">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b52ad-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b52ad-106">Prerequisites</span></span>
<span data-ttu-id="b52ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b52ad-109">Permission type</span></span>|<span data-ttu-id="b52ad-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b52ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b52ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b52ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b52ad-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52ad-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b52ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b52ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b52ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52ad-114">Not supported.</span></span>|
|<span data-ttu-id="b52ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b52ad-115">Application</span></span>|<span data-ttu-id="b52ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b52ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b52ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b52ad-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b52ad-118">Request headers</span></span>
|<span data-ttu-id="b52ad-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b52ad-119">Header</span></span>|<span data-ttu-id="b52ad-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b52ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b52ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b52ad-121">Authorization</span></span>|<span data-ttu-id="b52ad-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b52ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b52ad-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b52ad-123">Accept</span></span>|<span data-ttu-id="b52ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b52ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52ad-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b52ad-125">Request body</span></span>
<span data-ttu-id="b52ad-126">В теле запроса добавьте представление объекта [roleAssignment](../resources/intune-rbac-roleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b52ad-126">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="b52ad-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b52ad-127">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="b52ad-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b52ad-128">Property</span></span>|<span data-ttu-id="b52ad-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b52ad-129">Type</span></span>|<span data-ttu-id="b52ad-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b52ad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b52ad-131">id</span><span class="sxs-lookup"><span data-stu-id="b52ad-131">id</span></span>|<span data-ttu-id="b52ad-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b52ad-132">String</span></span>|<span data-ttu-id="b52ad-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b52ad-133">Key of the entity.</span></span> <span data-ttu-id="b52ad-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="b52ad-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b52ad-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b52ad-135">displayName</span></span>|<span data-ttu-id="b52ad-136">String</span><span class="sxs-lookup"><span data-stu-id="b52ad-136">String</span></span>|<span data-ttu-id="b52ad-137">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b52ad-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b52ad-138">описание</span><span class="sxs-lookup"><span data-stu-id="b52ad-138">description</span></span>|<span data-ttu-id="b52ad-139">String</span><span class="sxs-lookup"><span data-stu-id="b52ad-139">String</span></span>|<span data-ttu-id="b52ad-140">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b52ad-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b52ad-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b52ad-141">resourceScopes</span></span>|<span data-ttu-id="b52ad-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b52ad-142">String collection</span></span>|<span data-ttu-id="b52ad-143">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="b52ad-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b52ad-144">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b52ad-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b52ad-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52ad-145">Response</span></span>
<span data-ttu-id="b52ad-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [roleAssignment](../resources/intune-rbac-roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b52ad-146">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52ad-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b52ad-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b52ad-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b52ad-148">Request</span></span>
<span data-ttu-id="b52ad-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b52ad-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b52ad-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="b52ad-150">Response</span></span>
<span data-ttu-id="b52ad-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b52ad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



