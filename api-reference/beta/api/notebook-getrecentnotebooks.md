---
title: 'notebook: getRecentNotebooks'
description: Получите список экземпляров recentNotebook, которые недавно открывал вошедший в систему пользователь.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 98cd3631ccf62d7ea20f7bfe5bf53a4101c5e6d0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721721"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="b625a-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="b625a-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="b625a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b625a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b625a-105">Получите список экземпляров [recentNotebook](../resources/recentnotebook.md), которые недавно открывал вошедший в систему пользователь.</span><span class="sxs-lookup"><span data-stu-id="b625a-105">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b625a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b625a-106">Permissions</span></span>
<span data-ttu-id="b625a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b625a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b625a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b625a-109">Permission type</span></span>      | <span data-ttu-id="b625a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b625a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b625a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b625a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b625a-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b625a-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="b625a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b625a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b625a-114">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b625a-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="b625a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b625a-115">Application</span></span> | <span data-ttu-id="b625a-116">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b625a-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b625a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b625a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="b625a-118">Идентификатор `{id | userPrincipalName}` должен соответствовать пользователю, закодированному в токене авторизации, используемом для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="b625a-118">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="b625a-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b625a-119">Function parameters</span></span>

| <span data-ttu-id="b625a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="b625a-120">Parameter</span></span>    | <span data-ttu-id="b625a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b625a-121">Type</span></span>   |<span data-ttu-id="b625a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b625a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b625a-123">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="b625a-123">includePersonalNotebooks</span></span>|<span data-ttu-id="b625a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b625a-124">Boolean</span></span>|<span data-ttu-id="b625a-125">Включите записные книжки, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="b625a-125">Include notebooks owned by the user.</span></span> <span data-ttu-id="b625a-126">Установите значение `true`, чтобы включить записные книжки, принадлежащие пользователю; в противном случае установите значение `false`.</span><span class="sxs-lookup"><span data-stu-id="b625a-126">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="b625a-127">Если вы не включите параметр `includePersonalNotebooks`, запрос вернет ошибку `400`.</span><span class="sxs-lookup"><span data-stu-id="b625a-127">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b625a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b625a-128">Request headers</span></span>
| <span data-ttu-id="b625a-129">Имя</span><span class="sxs-lookup"><span data-stu-id="b625a-129">Name</span></span>       | <span data-ttu-id="b625a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b625a-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b625a-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b625a-131">Authorization</span></span>  | <span data-ttu-id="b625a-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b625a-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b625a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b625a-133">Request body</span></span>
<span data-ttu-id="b625a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b625a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b625a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b625a-135">Response</span></span>
<span data-ttu-id="b625a-136">В случае успеха возвращается ответ с кодом `200 OK`, который содержит JSON-коллекцию ресурсов **recentNotebook**.</span><span class="sxs-lookup"><span data-stu-id="b625a-136">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="b625a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b625a-137">Example</span></span>
<span data-ttu-id="b625a-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b625a-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b625a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b625a-139">Request</span></span>
<span data-ttu-id="b625a-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b625a-140">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="b625a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b625a-141">Response</span></span>
<span data-ttu-id="b625a-142">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b625a-142">The following example shows the response.</span></span>

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


