---
title: Создание программы
description: В функции рецензирования Access Azure AD создайте объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f48cb663a28bc5c82c4c1a78877d19ebd72364e9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412553"
---
# <a name="create-program"></a><span data-ttu-id="e537e-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="e537e-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e537e-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD создайте объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="e537e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e537e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e537e-105">Permissions</span></span>
<span data-ttu-id="e537e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e537e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e537e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e537e-108">Permission type</span></span>                        | <span data-ttu-id="e537e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e537e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e537e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e537e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e537e-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e537e-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="e537e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e537e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e537e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e537e-113">Not supported.</span></span> |
|<span data-ttu-id="e537e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e537e-114">Application</span></span>                            | <span data-ttu-id="e537e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e537e-115">Not supported.</span></span> |

<span data-ttu-id="e537e-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="e537e-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="e537e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e537e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="e537e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e537e-118">Request headers</span></span>
| <span data-ttu-id="e537e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e537e-119">Name</span></span>         | <span data-ttu-id="e537e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e537e-120">Type</span></span>        | <span data-ttu-id="e537e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e537e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e537e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e537e-122">Authorization</span></span> | <span data-ttu-id="e537e-123">string</span><span class="sxs-lookup"><span data-stu-id="e537e-123">string</span></span> | <span data-ttu-id="e537e-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e537e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e537e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e537e-126">Request body</span></span>
<span data-ttu-id="e537e-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e537e-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="e537e-128">В следующей таблице приведены свойства, необходимые при создании программы.</span><span class="sxs-lookup"><span data-stu-id="e537e-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="e537e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e537e-129">Property</span></span>     | <span data-ttu-id="e537e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e537e-130">Type</span></span>        | <span data-ttu-id="e537e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e537e-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="e537e-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="e537e-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="e537e-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="e537e-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="e537e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e537e-134">Response</span></span>
<span data-ttu-id="e537e-135">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e537e-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e537e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e537e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e537e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e537e-137">Request</span></span>
<span data-ttu-id="e537e-138">В тексте запроса добавьте представление объекта [Program](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e537e-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e537e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e537e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e537e-140">C#</span><span class="sxs-lookup"><span data-stu-id="e537e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-program-from-programs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e537e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e537e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-program-from-programs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e537e-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e537e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-program-from-programs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e537e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e537e-143">Response</span></span>
><span data-ttu-id="e537e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e537e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="e537e-146">См. также</span><span class="sxs-lookup"><span data-stu-id="e537e-146">See also</span></span>

| <span data-ttu-id="e537e-147">Метод</span><span class="sxs-lookup"><span data-stu-id="e537e-147">Method</span></span>           | <span data-ttu-id="e537e-148">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e537e-148">Return Type</span></span>    |<span data-ttu-id="e537e-149">Описание</span><span class="sxs-lookup"><span data-stu-id="e537e-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e537e-150">Список программ</span><span class="sxs-lookup"><span data-stu-id="e537e-150">List programs</span></span>](program-list.md) | <span data-ttu-id="e537e-151">Коллекция [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="e537e-151">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="e537e-152">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="e537e-152">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="e537e-153">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="e537e-153">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="e537e-154">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="e537e-154">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="e537e-155">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="e537e-155">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="e537e-156">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="e537e-156">Update program</span></span>](program-update.md) |  [<span data-ttu-id="e537e-157">Программа</span><span class="sxs-lookup"><span data-stu-id="e537e-157">program</span></span>](../resources/program.md)| <span data-ttu-id="e537e-158">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="e537e-158">Update a program.</span></span>|
|[<span data-ttu-id="e537e-159">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="e537e-159">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="e537e-160">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="e537e-160">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="e537e-161">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="e537e-161">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
