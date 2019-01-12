---
title: 'notebook: getRecentNotebooks'
description: Получите список экземпляров recentNotebook, которые недавно открывал вошедший в систему пользователь.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 31f95d8e94ef22c6b0cbea1cbb5ff8b98c58d187
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931673"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="7aef7-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="7aef7-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="7aef7-104">Получите список экземпляров [recentNotebook](../resources/recentnotebook.md), которые недавно открывал вошедший в систему пользователь.</span><span class="sxs-lookup"><span data-stu-id="7aef7-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aef7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aef7-105">Permissions</span></span>
<span data-ttu-id="7aef7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aef7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aef7-108">Permission type</span></span>      | <span data-ttu-id="7aef7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aef7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aef7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aef7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aef7-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aef7-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="7aef7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aef7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aef7-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aef7-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="7aef7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aef7-114">Application</span></span> | <span data-ttu-id="7aef7-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aef7-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aef7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aef7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="7aef7-117">Идентификатор `<id | userPrincipalName>` должен соответствовать пользователю, закодированному в токене авторизации, используемом для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="7aef7-117">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="7aef7-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="7aef7-118">Function parameters</span></span>

| <span data-ttu-id="7aef7-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="7aef7-119">Parameter</span></span>    | <span data-ttu-id="7aef7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7aef7-120">Type</span></span>   |<span data-ttu-id="7aef7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7aef7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aef7-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="7aef7-122">includePersonalNotebooks</span></span>|<span data-ttu-id="7aef7-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="7aef7-123">Boolean</span></span>|<span data-ttu-id="7aef7-124">Включите записные книжки, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="7aef7-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="7aef7-125">Установите значение `true`, чтобы включить записные книжки, принадлежащие пользователю; в противном случае установите значение `false`.</span><span class="sxs-lookup"><span data-stu-id="7aef7-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="7aef7-126">Если вы не включите параметр `includePersonalNotebooks`, запрос вернет ошибку `400`.</span><span class="sxs-lookup"><span data-stu-id="7aef7-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7aef7-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aef7-127">Request headers</span></span>
| <span data-ttu-id="7aef7-128">Имя</span><span class="sxs-lookup"><span data-stu-id="7aef7-128">Name</span></span>       | <span data-ttu-id="7aef7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7aef7-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7aef7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aef7-130">Authorization</span></span>  | <span data-ttu-id="7aef7-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7aef7-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aef7-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7aef7-132">Request body</span></span>
<span data-ttu-id="7aef7-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7aef7-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aef7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7aef7-134">Response</span></span>
<span data-ttu-id="7aef7-135">В случае успеха возвращается ответ с кодом `200 OK`, который содержит JSON-коллекцию ресурсов **recentNotebook**.</span><span class="sxs-lookup"><span data-stu-id="7aef7-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="7aef7-136">Пример</span><span class="sxs-lookup"><span data-stu-id="7aef7-136">Example</span></span>
<span data-ttu-id="7aef7-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7aef7-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7aef7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aef7-138">Request</span></span>
<span data-ttu-id="7aef7-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aef7-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="7aef7-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="7aef7-140">Response</span></span>
<span data-ttu-id="7aef7-141">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7aef7-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
