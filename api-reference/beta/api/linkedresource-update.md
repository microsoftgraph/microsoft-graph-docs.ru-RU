---
title: Обновление linkedResource
description: Обновление свойств объекта linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b87170c634f1bd0a95bfac6118f97554426f2ecb
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850083"
---
# <a name="update-linkedresource"></a><span data-ttu-id="ab06c-103">Обновление linkedResource</span><span class="sxs-lookup"><span data-stu-id="ab06c-103">Update linkedResource</span></span>
<span data-ttu-id="ab06c-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="ab06c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="ab06c-105">Обновление свойств объекта [linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="ab06c-105">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab06c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab06c-106">Permissions</span></span>
<span data-ttu-id="ab06c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab06c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab06c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab06c-109">Permission type</span></span>|<span data-ttu-id="ab06c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab06c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab06c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab06c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab06c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab06c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ab06c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab06c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab06c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab06c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ab06c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab06c-115">Application</span></span>|<span data-ttu-id="ab06c-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ab06c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab06c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab06c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="ab06c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab06c-118">Request headers</span></span>
|<span data-ttu-id="ab06c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ab06c-119">Name</span></span>|<span data-ttu-id="ab06c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ab06c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ab06c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab06c-121">Authorization</span></span>|<span data-ttu-id="ab06c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab06c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ab06c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab06c-124">Content-Type</span></span>|<span data-ttu-id="ab06c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab06c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab06c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab06c-127">Request body</span></span>
<span data-ttu-id="ab06c-128">Представьте в тексте запроса описание объекта [linkedResource в формате](../resources/linkedresource.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="ab06c-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="ab06c-129">В приведенной ниже таблице указаны свойства, необходимые при обновлении [ресурса linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="ab06c-129">The following table shows the properties that are required when you update the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="ab06c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab06c-130">Property</span></span>|<span data-ttu-id="ab06c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab06c-131">Type</span></span>|<span data-ttu-id="ab06c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab06c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab06c-133">id</span><span class="sxs-lookup"><span data-stu-id="ab06c-133">id</span></span>|<span data-ttu-id="ab06c-134">String</span><span class="sxs-lookup"><span data-stu-id="ab06c-134">String</span></span>|<span data-ttu-id="ab06c-135">Сгенерированный сервером ИД связанной сущности. Наследуется от [объекта.](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="ab06c-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="response"></a><span data-ttu-id="ab06c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab06c-136">Response</span></span>

<span data-ttu-id="ab06c-137">При успешном выполнении этот метод возвращает код `200 OK` ответа и [обновленный объект linkedResource](../resources/linkedresource.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ab06c-137">If successful, this method returns a `200 OK` response code and an updated [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab06c-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ab06c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab06c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab06c-139">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "update_linkedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
}
```

### <a name="response"></a><span data-ttu-id="ab06c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab06c-140">Response</span></span>
<span data-ttu-id="ab06c-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ab06c-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```