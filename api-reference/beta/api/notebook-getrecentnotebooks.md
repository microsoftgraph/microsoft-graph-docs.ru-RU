---
title: 'notebook: getRecentNotebooks'
description: Получите список экземпляров recentNotebook, которые недавно открывал вошедший в систему пользователь.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0487a7810602f709ea6386957fa1047a60111990
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887327"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="4075d-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="4075d-103">notebook: getRecentNotebooks</span></span>

> <span data-ttu-id="4075d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4075d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4075d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4075d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4075d-106">Получите список экземпляров [recentNotebook](../resources/recentnotebook.md), которые недавно открывал вошедший в систему пользователь.</span><span class="sxs-lookup"><span data-stu-id="4075d-106">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4075d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4075d-107">Permissions</span></span>
<span data-ttu-id="4075d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4075d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4075d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4075d-110">Permission type</span></span>      | <span data-ttu-id="4075d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4075d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4075d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4075d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4075d-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4075d-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="4075d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4075d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4075d-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4075d-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="4075d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4075d-116">Application</span></span> | <span data-ttu-id="4075d-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4075d-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4075d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4075d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="4075d-119">Идентификатор `<id | userPrincipalName>` должен соответствовать пользователю, закодированному в токене авторизации, используемом для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="4075d-119">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="4075d-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="4075d-120">Function parameters</span></span>

| <span data-ttu-id="4075d-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="4075d-121">Parameter</span></span>    | <span data-ttu-id="4075d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4075d-122">Type</span></span>   |<span data-ttu-id="4075d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4075d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4075d-124">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="4075d-124">includePersonalNotebooks</span></span>|<span data-ttu-id="4075d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4075d-125">Boolean</span></span>|<span data-ttu-id="4075d-126">Включите записные книжки, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="4075d-126">Include notebooks owned by the user.</span></span> <span data-ttu-id="4075d-127">Установите значение `true`, чтобы включить записные книжки, принадлежащие пользователю; в противном случае установите значение `false`.</span><span class="sxs-lookup"><span data-stu-id="4075d-127">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="4075d-128">Если вы не включите параметр `includePersonalNotebooks`, запрос вернет ошибку `400`.</span><span class="sxs-lookup"><span data-stu-id="4075d-128">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4075d-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4075d-129">Request headers</span></span>
| <span data-ttu-id="4075d-130">Имя</span><span class="sxs-lookup"><span data-stu-id="4075d-130">Name</span></span>       | <span data-ttu-id="4075d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4075d-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4075d-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4075d-132">Authorization</span></span>  | <span data-ttu-id="4075d-133">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4075d-133">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4075d-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4075d-134">Request body</span></span>
<span data-ttu-id="4075d-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4075d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4075d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4075d-136">Response</span></span>
<span data-ttu-id="4075d-137">В случае успеха возвращается ответ с кодом `200 OK`, который содержит JSON-коллекцию ресурсов **recentNotebook**.</span><span class="sxs-lookup"><span data-stu-id="4075d-137">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="4075d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4075d-138">Example</span></span>
<span data-ttu-id="4075d-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4075d-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4075d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4075d-140">Request</span></span>
<span data-ttu-id="4075d-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4075d-141">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="4075d-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="4075d-142">Response</span></span>
<span data-ttu-id="4075d-143">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4075d-143">The following example shows the response.</span></span>

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
