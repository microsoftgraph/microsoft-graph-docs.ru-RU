---
title: 'notebook: getRecentNotebooks'
description: Получите список экземпляров recentNotebook, которые недавно открывал вошедший в систему пользователь.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 0ed8765dd5162d95932be6c4556b986579f9af1b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338231"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="b3e2b-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="b3e2b-103">notebook: getRecentNotebooks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e2b-104">Получите список экземпляров [recentNotebook](../resources/recentnotebook.md), которые недавно открывал вошедший в систему пользователь.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3e2b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3e2b-105">Permissions</span></span>
<span data-ttu-id="b3e2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3e2b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3e2b-108">Permission type</span></span>      | <span data-ttu-id="b3e2b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3e2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3e2b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3e2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3e2b-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e2b-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="b3e2b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3e2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3e2b-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3e2b-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="b3e2b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3e2b-114">Application</span></span> | <span data-ttu-id="b3e2b-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3e2b-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3e2b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3e2b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="b3e2b-117">Идентификатор `{id | userPrincipalName}` должен соответствовать пользователю, закодированному в токене авторизации, используемом для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-117">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="b3e2b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b3e2b-118">Function parameters</span></span>

| <span data-ttu-id="b3e2b-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="b3e2b-119">Parameter</span></span>    | <span data-ttu-id="b3e2b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b3e2b-120">Type</span></span>   |<span data-ttu-id="b3e2b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b3e2b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3e2b-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="b3e2b-122">includePersonalNotebooks</span></span>|<span data-ttu-id="b3e2b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3e2b-123">Boolean</span></span>|<span data-ttu-id="b3e2b-124">Включите записные книжки, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="b3e2b-125">Установите значение `true`, чтобы включить записные книжки, принадлежащие пользователю; в противном случае установите значение `false`.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="b3e2b-126">Если вы не включите параметр `includePersonalNotebooks`, запрос вернет ошибку `400`.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b3e2b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3e2b-127">Request headers</span></span>
| <span data-ttu-id="b3e2b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b3e2b-128">Name</span></span>       | <span data-ttu-id="b3e2b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b3e2b-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3e2b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3e2b-130">Authorization</span></span>  | <span data-ttu-id="b3e2b-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b3e2b-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3e2b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3e2b-132">Request body</span></span>
<span data-ttu-id="b3e2b-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3e2b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3e2b-134">Response</span></span>
<span data-ttu-id="b3e2b-135">В случае успеха возвращается ответ с кодом `200 OK`, который содержит JSON-коллекцию ресурсов **recentNotebook**.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="b3e2b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b3e2b-136">Example</span></span>
<span data-ttu-id="b3e2b-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b3e2b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3e2b-138">Request</span></span>
<span data-ttu-id="b3e2b-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="b3e2b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3e2b-140">Response</span></span>
<span data-ttu-id="b3e2b-141">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
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
