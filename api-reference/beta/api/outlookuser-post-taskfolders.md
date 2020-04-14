---
title: Создание outlookTaskFolder
description: Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 63662dffac9cb36031efd11cac76eb8bd23b0da1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456202"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="5d654-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="5d654-103">Create outlookTaskFolder</span></span>

<span data-ttu-id="5d654-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d654-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d654-105">Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d654-105">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d654-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d654-106">Permissions</span></span>
<span data-ttu-id="5d654-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d654-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d654-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d654-109">Permission type</span></span>      | <span data-ttu-id="5d654-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d654-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d654-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d654-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d654-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d654-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5d654-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d654-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d654-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d654-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5d654-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d654-115">Application</span></span> | <span data-ttu-id="5d654-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d654-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d654-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d654-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="5d654-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d654-118">Request headers</span></span>
| <span data-ttu-id="5d654-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5d654-119">Name</span></span>       | <span data-ttu-id="5d654-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5d654-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d654-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d654-121">Authorization</span></span>  | <span data-ttu-id="5d654-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d654-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d654-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d654-124">Request body</span></span>
<span data-ttu-id="5d654-125">В тексте запроса добавьте представление объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d654-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5d654-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d654-126">Response</span></span>

<span data-ttu-id="5d654-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d654-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d654-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5d654-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d654-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d654-129">Request</span></span>
<span data-ttu-id="5d654-130">В следующем примере создается папка Task с именем "добровольный" в группе задач`My Tasks`по умолчанию () почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d654-130">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d654-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d654-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5d654-132">C#</span><span class="sxs-lookup"><span data-stu-id="5d654-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d654-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d654-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d654-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d654-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5d654-135">В тексте запроса добавьте представление объекта [outlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d654-135">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5d654-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d654-136">Response</span></span>
<span data-ttu-id="5d654-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d654-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
