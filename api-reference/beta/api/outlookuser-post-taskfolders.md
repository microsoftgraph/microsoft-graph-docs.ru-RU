---
title: Создание outlookTaskFolder
description: Создайте папку задач в группе задач по умолчанию `My Tasks` () почтового ящика пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9aafda49a7d02169c791c4038195aca4d387928b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038007"
---
# <a name="create-outlooktaskfolder-deprecated"></a><span data-ttu-id="34401-103">Создание outlookTaskFolder (амортизации)</span><span class="sxs-lookup"><span data-stu-id="34401-103">Create outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="34401-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="34401-105">Создайте папку задач в группе задач по умолчанию `My Tasks` () почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="34401-105">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="34401-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34401-106">Permissions</span></span>
<span data-ttu-id="34401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34401-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34401-109">Permission type</span></span>      | <span data-ttu-id="34401-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34401-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34401-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="34401-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34401-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="34401-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34401-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34401-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="34401-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34401-115">Application</span></span> | <span data-ttu-id="34401-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34401-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34401-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34401-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="34401-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34401-118">Request headers</span></span>
| <span data-ttu-id="34401-119">Имя</span><span class="sxs-lookup"><span data-stu-id="34401-119">Name</span></span>       | <span data-ttu-id="34401-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34401-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34401-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34401-121">Authorization</span></span>  | <span data-ttu-id="34401-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34401-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34401-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34401-124">Request body</span></span>
<span data-ttu-id="34401-125">В теле запроса поставляем представление JSON объекта [OutlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="34401-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="34401-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="34401-126">Response</span></span>

<span data-ttu-id="34401-127">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект OutlookTaskFolder](../resources/outlooktaskfolder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="34401-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34401-128">Пример</span><span class="sxs-lookup"><span data-stu-id="34401-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34401-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="34401-129">Request</span></span>
<span data-ttu-id="34401-130">В следующем примере создается папка задач под названием Volunteer в целевой группе по умолчанию () почтового `My Tasks` ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="34401-130">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="34401-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="34401-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
# <a name="c"></a>[<span data-ttu-id="34401-132">C#</span><span class="sxs-lookup"><span data-stu-id="34401-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34401-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34401-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34401-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34401-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34401-135">Java</span><span class="sxs-lookup"><span data-stu-id="34401-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktaskfolder-from-outlookuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="34401-136">В теле запроса поставляем представление JSON объекта [OutlookTaskFolder.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="34401-136">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="34401-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="34401-137">Response</span></span>
<span data-ttu-id="34401-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34401-138">Here is an example of the response.</span></span> <span data-ttu-id="34401-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="34401-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


