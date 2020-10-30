---
title: Список Линкедресаурцес
description: Получение Линкедресаурцес из свойства навигации Линкедресаурцес.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 04c0ca76b3d3d8c09fcec126a95aa75a8ba774e3
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797339"
---
# <a name="list-linkedresources"></a><span data-ttu-id="ba090-103">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="ba090-103">List linkedResources</span></span>
<span data-ttu-id="ba090-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba090-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba090-105">Получение сведений об одном или нескольких элементах партнерского приложения, на основе которого была создана указанная [задача](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="ba090-105">Get information of one or more items in a partner application, based on which a specified [task](../resources/todotask.md) was created.</span></span> <span data-ttu-id="ba090-106">Сведения представлены в объекте [линкедресаурце](../resources/linkedresource.md) для каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="ba090-106">The information is represented in a [linkedResource](../resources/linkedresource.md) object for each item.</span></span> <span data-ttu-id="ba090-107">Он включает внешний идентификатор элемента в партнерской приложении и, если это возможно, глубокая ссылка на этот элемент в приложении.</span><span class="sxs-lookup"><span data-stu-id="ba090-107">It includes an external ID for the item in the partner application, and if applicable, a deep link to that item in the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba090-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba090-108">Permissions</span></span>
<span data-ttu-id="ba090-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba090-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba090-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba090-111">Permission type</span></span>|<span data-ttu-id="ba090-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba090-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba090-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba090-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba090-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba090-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ba090-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba090-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba090-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba090-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="ba090-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba090-117">Application</span></span>|<span data-ttu-id="ba090-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba090-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba090-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba090-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba090-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba090-120">Optional query parameters</span></span>
<span data-ttu-id="ba090-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ba090-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba090-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ba090-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba090-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba090-123">Request headers</span></span>
|<span data-ttu-id="ba090-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ba090-124">Name</span></span>|<span data-ttu-id="ba090-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ba090-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba090-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba090-126">Authorization</span></span>|<span data-ttu-id="ba090-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba090-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba090-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba090-129">Request body</span></span>
<span data-ttu-id="ba090-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba090-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba090-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba090-131">Response</span></span>

<span data-ttu-id="ba090-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [линкедресаурце](../resources/linkedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba090-132">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba090-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba090-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba090-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba090-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```


### <a name="response"></a><span data-ttu-id="ba090-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba090-135">Response</span></span>
<span data-ttu-id="ba090-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba090-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.linkedResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http:://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
    }
  ]
}
```



