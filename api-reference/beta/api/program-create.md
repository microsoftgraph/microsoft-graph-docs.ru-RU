---
title: Создание программы
description: В функции рецензирования Access Azure AD создайте объект программы.
localization_priority: Normal
ms.openlocfilehash: 87f766917499e6e9d1896ccf64f8fbae2bef813b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593678"
---
# <a name="create-program"></a><span data-ttu-id="c751a-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="c751a-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c751a-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD создайте объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="c751a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c751a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c751a-105">Permissions</span></span>
<span data-ttu-id="c751a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c751a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c751a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c751a-108">Permission type</span></span>                        | <span data-ttu-id="c751a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c751a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c751a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c751a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c751a-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c751a-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="c751a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c751a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c751a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c751a-113">Not supported.</span></span> |
|<span data-ttu-id="c751a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c751a-114">Application</span></span>                            | <span data-ttu-id="c751a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c751a-115">Not supported.</span></span> |

<span data-ttu-id="c751a-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="c751a-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="c751a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c751a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="c751a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c751a-118">Request headers</span></span>
| <span data-ttu-id="c751a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c751a-119">Name</span></span>         | <span data-ttu-id="c751a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c751a-120">Type</span></span>        | <span data-ttu-id="c751a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c751a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c751a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c751a-122">Authorization</span></span> | <span data-ttu-id="c751a-123">string</span><span class="sxs-lookup"><span data-stu-id="c751a-123">string</span></span> | <span data-ttu-id="c751a-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c751a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c751a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c751a-126">Request body</span></span>
<span data-ttu-id="c751a-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c751a-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="c751a-128">В следующей таблице приведены свойства, необходимые при создании программы.</span><span class="sxs-lookup"><span data-stu-id="c751a-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="c751a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c751a-129">Property</span></span>     | <span data-ttu-id="c751a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c751a-130">Type</span></span>        | <span data-ttu-id="c751a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c751a-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="c751a-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="c751a-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="c751a-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="c751a-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="c751a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c751a-134">Response</span></span>
<span data-ttu-id="c751a-135">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c751a-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c751a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c751a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c751a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c751a-137">Request</span></span>
<span data-ttu-id="c751a-138">В тексте запроса добавьте представление объекта [Program](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c751a-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c751a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c751a-139">Response</span></span>
><span data-ttu-id="c751a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c751a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c751a-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c751a-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c751a-143">Языках</span><span class="sxs-lookup"><span data-stu-id="c751a-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c751a-144">Язык</span><span class="sxs-lookup"><span data-stu-id="c751a-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_program_from_programs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="c751a-145">См. также</span><span class="sxs-lookup"><span data-stu-id="c751a-145">See also</span></span>

| <span data-ttu-id="c751a-146">Метод</span><span class="sxs-lookup"><span data-stu-id="c751a-146">Method</span></span>           | <span data-ttu-id="c751a-147">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c751a-147">Return Type</span></span>    |<span data-ttu-id="c751a-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c751a-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c751a-149">Список программ</span><span class="sxs-lookup"><span data-stu-id="c751a-149">List programs</span></span>](program-list.md) | <span data-ttu-id="c751a-150">Коллекция [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="c751a-150">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="c751a-151">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="c751a-151">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="c751a-152">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="c751a-152">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="c751a-153">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="c751a-153">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="c751a-154">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="c751a-154">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="c751a-155">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="c751a-155">Update program</span></span>](program-update.md) |  [<span data-ttu-id="c751a-156">Программа</span><span class="sxs-lookup"><span data-stu-id="c751a-156">program</span></span>](../resources/program.md)| <span data-ttu-id="c751a-157">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="c751a-157">Update a program.</span></span>|
|[<span data-ttu-id="c751a-158">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c751a-158">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="c751a-159">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c751a-159">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="c751a-160">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="c751a-160">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
