---
title: Создание Линкедресаурцес
description: Создание нового объекта Линкедресаурцес.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4311af292480a51eeaaefabb1ef8cf277b211e2c
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873251"
---
# <a name="create-linkedresources"></a><span data-ttu-id="eeb6c-103">Создание Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="eeb6c-103">Create linkedResources</span></span>
<span data-ttu-id="eeb6c-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="eeb6c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="eeb6c-105">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-105">Create a new linkedResources object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eeb6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb6c-106">Permissions</span></span>
<span data-ttu-id="eeb6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeb6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb6c-109">Permission type</span></span>|<span data-ttu-id="eeb6c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeb6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeb6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeb6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eeb6c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb6c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="eeb6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeb6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeb6c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb6c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="eeb6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeb6c-115">Application</span></span>|<span data-ttu-id="eeb6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeb6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeb6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="eeb6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eeb6c-118">Request headers</span></span>
|<span data-ttu-id="eeb6c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eeb6c-119">Name</span></span>|<span data-ttu-id="eeb6c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb6c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eeb6c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeb6c-121">Authorization</span></span>|<span data-ttu-id="eeb6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eeb6c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eeb6c-124">Content-Type</span></span>|<span data-ttu-id="eeb6c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeb6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eeb6c-127">Request body</span></span>
<span data-ttu-id="eeb6c-128">В тексте запроса добавьте представление объекта [линкедресаурце](../resources/linkedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="eeb6c-129">В следующей таблице приведены свойства, необходимые при создании [линкедресаурце](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="eeb6c-129">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="eeb6c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeb6c-130">Property</span></span>|<span data-ttu-id="eeb6c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eeb6c-131">Type</span></span>|<span data-ttu-id="eeb6c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeb6c-133">id</span><span class="sxs-lookup"><span data-stu-id="eeb6c-133">id</span></span>|<span data-ttu-id="eeb6c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="eeb6c-134">String</span></span>|<span data-ttu-id="eeb6c-135">Созданный сервером идентификатор связанной сущности, унаследованной от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="eeb6c-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="eeb6c-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="eeb6c-136">webUrl</span></span>|<span data-ttu-id="eeb6c-137">String</span><span class="sxs-lookup"><span data-stu-id="eeb6c-137">String</span></span>|<span data-ttu-id="eeb6c-138">Прямой ссылки на связанный объект</span><span class="sxs-lookup"><span data-stu-id="eeb6c-138">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="eeb6c-139">applicationName</span><span class="sxs-lookup"><span data-stu-id="eeb6c-139">applicationName</span></span>|<span data-ttu-id="eeb6c-140">String</span><span class="sxs-lookup"><span data-stu-id="eeb6c-140">String</span></span>|<span data-ttu-id="eeb6c-141">Поле, указывающее имя приложения источника, отправляющего связанный объект</span><span class="sxs-lookup"><span data-stu-id="eeb6c-141">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="eeb6c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="eeb6c-142">displayName</span></span>|<span data-ttu-id="eeb6c-143">Строка</span><span class="sxs-lookup"><span data-stu-id="eeb6c-143">String</span></span>|<span data-ttu-id="eeb6c-144">Поле, указывающее название связанного объекта.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-144">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="eeb6c-145">externalId</span><span class="sxs-lookup"><span data-stu-id="eeb6c-145">externalId</span></span>|<span data-ttu-id="eeb6c-146">String</span><span class="sxs-lookup"><span data-stu-id="eeb6c-146">String</span></span>|<span data-ttu-id="eeb6c-147">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="eeb6c-147">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="eeb6c-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="eeb6c-148">Response</span></span>

<span data-ttu-id="eeb6c-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-149">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eeb6c-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="eeb6c-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eeb6c-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeb6c-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eeb6c-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="eeb6c-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="eeb6c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eeb6c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eeb6c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeb6c-154">Response</span></span>
<span data-ttu-id="eeb6c-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eeb6c-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```

