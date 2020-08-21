---
title: Создание объекта outlookTaskFolder
description: Создайте папку задач в группе задач по умолчанию `My Tasks` () почтового ящика пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7f1c1767f125da2745837addb7852805630f5231
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849319"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="0ac8f-103">Создание объекта outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="0ac8f-103">Create outlookTaskFolder</span></span>

<span data-ttu-id="0ac8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ac8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="0ac8f-105">Создайте папку задач в группе задач по умолчанию `My Tasks` () почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-105">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac8f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ac8f-106">Permissions</span></span>
<span data-ttu-id="0ac8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ac8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac8f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ac8f-109">Permission type</span></span>      | <span data-ttu-id="0ac8f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ac8f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ac8f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ac8f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ac8f-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac8f-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0ac8f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ac8f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac8f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac8f-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0ac8f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ac8f-115">Application</span></span> | <span data-ttu-id="0ac8f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ac8f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ac8f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="0ac8f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ac8f-118">Request headers</span></span>
| <span data-ttu-id="0ac8f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ac8f-119">Name</span></span>       | <span data-ttu-id="0ac8f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac8f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ac8f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ac8f-121">Authorization</span></span>  | <span data-ttu-id="0ac8f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ac8f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ac8f-124">Request body</span></span>
<span data-ttu-id="0ac8f-125">Представьте в тексте запроса описание объекта [outlookTaskFolder в формате](../resources/outlooktaskfolder.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-125">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0ac8f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ac8f-126">Response</span></span>

<span data-ttu-id="0ac8f-127">При успешном выполнении этот метод возвращает `201 Created` код ответа [и объект outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-127">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac8f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0ac8f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ac8f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ac8f-129">Request</span></span>
<span data-ttu-id="0ac8f-130">В следующем примере создается папка задач "Волонтер" в группе задач по умолчанию `My Tasks` () почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-130">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ac8f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ac8f-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ac8f-132">C#</span><span class="sxs-lookup"><span data-stu-id="0ac8f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktaskfolder-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ac8f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ac8f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktaskfolder-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ac8f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ac8f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktaskfolder-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0ac8f-135">Представьте в тексте запроса описание объекта [outlookTaskFolder в формате](../resources/outlooktaskfolder.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-135">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0ac8f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ac8f-136">Response</span></span>
<span data-ttu-id="0ac8f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ac8f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
