---
title: Создание linkedResources
description: Создание объекта linkedResources.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5180b5a38dafceb30871e574208d5321c8b0c38c
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850066"
---
# <a name="create-linkedresources"></a><span data-ttu-id="5ffa9-103">Создание linkedResources</span><span class="sxs-lookup"><span data-stu-id="5ffa9-103">Create linkedResources</span></span>
<span data-ttu-id="5ffa9-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="5ffa9-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="5ffa9-105">Создание объекта linkedResources.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-105">Create a new linkedResources object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ffa9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ffa9-106">Permissions</span></span>
<span data-ttu-id="5ffa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ffa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ffa9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ffa9-109">Permission type</span></span>|<span data-ttu-id="5ffa9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ffa9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ffa9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ffa9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ffa9-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ffa9-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="5ffa9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ffa9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ffa9-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ffa9-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="5ffa9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ffa9-115">Application</span></span>|<span data-ttu-id="5ffa9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ffa9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ffa9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="5ffa9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ffa9-118">Request headers</span></span>
|<span data-ttu-id="5ffa9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5ffa9-119">Name</span></span>|<span data-ttu-id="5ffa9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5ffa9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ffa9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ffa9-121">Authorization</span></span>|<span data-ttu-id="5ffa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5ffa9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ffa9-124">Content-Type</span></span>|<span data-ttu-id="5ffa9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ffa9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ffa9-127">Request body</span></span>
<span data-ttu-id="5ffa9-128">Представьте в тексте запроса описание объекта [linkedResource в формате](../resources/linkedresource.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="5ffa9-129">В приведенной ниже таблице указаны свойства, необходимые при создании [объекта linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="5ffa9-129">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="5ffa9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ffa9-130">Property</span></span>|<span data-ttu-id="5ffa9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5ffa9-131">Type</span></span>|<span data-ttu-id="5ffa9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5ffa9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ffa9-133">id</span><span class="sxs-lookup"><span data-stu-id="5ffa9-133">id</span></span>|<span data-ttu-id="5ffa9-134">String</span><span class="sxs-lookup"><span data-stu-id="5ffa9-134">String</span></span>|<span data-ttu-id="5ffa9-135">Сгенерированный сервером ИД связанной сущности. Наследуется от [объекта.](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="5ffa9-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="5ffa9-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="5ffa9-136">webUrl</span></span>|<span data-ttu-id="5ffa9-137">String</span><span class="sxs-lookup"><span data-stu-id="5ffa9-137">String</span></span>|<span data-ttu-id="5ffa9-138">Глубокая ссылка на связанный объект</span><span class="sxs-lookup"><span data-stu-id="5ffa9-138">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="5ffa9-139">applicationName</span><span class="sxs-lookup"><span data-stu-id="5ffa9-139">applicationName</span></span>|<span data-ttu-id="5ffa9-140">String</span><span class="sxs-lookup"><span data-stu-id="5ffa9-140">String</span></span>|<span data-ttu-id="5ffa9-141">Поле, указывающее имя приложения источника, отправляющего связанную сущность</span><span class="sxs-lookup"><span data-stu-id="5ffa9-141">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="5ffa9-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5ffa9-142">displayName</span></span>|<span data-ttu-id="5ffa9-143">String</span><span class="sxs-lookup"><span data-stu-id="5ffa9-143">String</span></span>|<span data-ttu-id="5ffa9-144">Поле, обозначающее заголовок связанной сущности.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-144">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="5ffa9-145">externalId</span><span class="sxs-lookup"><span data-stu-id="5ffa9-145">externalId</span></span>|<span data-ttu-id="5ffa9-146">String</span><span class="sxs-lookup"><span data-stu-id="5ffa9-146">String</span></span>|<span data-ttu-id="5ffa9-147">Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе</span><span class="sxs-lookup"><span data-stu-id="5ffa9-147">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="5ffa9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ffa9-148">Response</span></span>

<span data-ttu-id="5ffa9-149">При успешном выполнении этот метод возвращает `201 Created` код ответа [и объект linkedResource](../resources/linkedresource.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-149">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ffa9-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ffa9-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ffa9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ffa9-151">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="5ffa9-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ffa9-152">Response</span></span>
<span data-ttu-id="5ffa9-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5ffa9-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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

