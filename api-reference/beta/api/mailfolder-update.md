---
title: Обновление mailFolder
description: Обновление свойства объекта mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33e900933bc643f36e8f8a7783ea2083b3c03887
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976585"
---
# <a name="update-mailfolder"></a><span data-ttu-id="951e3-103">Обновление mailFolder</span><span class="sxs-lookup"><span data-stu-id="951e3-103">Update mailFolder</span></span>

> <span data-ttu-id="951e3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="951e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="951e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="951e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="951e3-106">Обновление свойства объекта [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="951e3-106">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="951e3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="951e3-107">Permissions</span></span>
<span data-ttu-id="951e3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="951e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="951e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="951e3-110">Permission type</span></span>      | <span data-ttu-id="951e3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="951e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="951e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="951e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="951e3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="951e3-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="951e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="951e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="951e3-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="951e3-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="951e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="951e3-116">Application</span></span> | <span data-ttu-id="951e3-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="951e3-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="951e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="951e3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="951e3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="951e3-119">Request headers</span></span>
| <span data-ttu-id="951e3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="951e3-120">Header</span></span>       | <span data-ttu-id="951e3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="951e3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="951e3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="951e3-122">Authorization</span></span>  | <span data-ttu-id="951e3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="951e3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="951e3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="951e3-125">Content-Type</span></span>  | <span data-ttu-id="951e3-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="951e3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="951e3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="951e3-128">Request body</span></span>
<span data-ttu-id="951e3-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="951e3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="951e3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="951e3-132">Property</span></span>     | <span data-ttu-id="951e3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="951e3-133">Type</span></span>   |<span data-ttu-id="951e3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="951e3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="951e3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="951e3-135">displayName</span></span>|<span data-ttu-id="951e3-136">Строка</span><span class="sxs-lookup"><span data-stu-id="951e3-136">String</span></span>|<span data-ttu-id="951e3-137">Отображаемое имя объекта mailFolder.</span><span class="sxs-lookup"><span data-stu-id="951e3-137">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="951e3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="951e3-138">Response</span></span>
<span data-ttu-id="951e3-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="951e3-139">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="951e3-140">Пример</span><span class="sxs-lookup"><span data-stu-id="951e3-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="951e3-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="951e3-141">Request</span></span>
<span data-ttu-id="951e3-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="951e3-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

#### <a name="response"></a><span data-ttu-id="951e3-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="951e3-143">Response</span></span>
<span data-ttu-id="951e3-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="951e3-144">The following is an example of the response.</span></span>
><span data-ttu-id="951e3-145">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="951e3-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="951e3-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="951e3-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
