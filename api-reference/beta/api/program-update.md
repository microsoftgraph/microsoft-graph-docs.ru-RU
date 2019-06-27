---
title: Программа обновления
description: В функции проверки доступа Azure AD обновите существующий объект программы.
localization_priority: Normal
ms.openlocfilehash: bc4971dd825b031d786d50aeffe3a96eb5a7ef80
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264101"
---
# <a name="update-program"></a><span data-ttu-id="c4901-103">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="c4901-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4901-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="c4901-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4901-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4901-105">Permissions</span></span>
<span data-ttu-id="c4901-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4901-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4901-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4901-108">Permission type</span></span>                        | <span data-ttu-id="c4901-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4901-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4901-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4901-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4901-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4901-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="c4901-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4901-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4901-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4901-113">Not supported.</span></span> |
|<span data-ttu-id="c4901-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4901-114">Application</span></span>                            | <span data-ttu-id="c4901-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4901-115">Not supported.</span></span> |

<span data-ttu-id="c4901-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им обновлять программу.</span><span class="sxs-lookup"><span data-stu-id="c4901-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="c4901-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4901-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="c4901-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4901-118">Request headers</span></span>
| <span data-ttu-id="c4901-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4901-119">Name</span></span>         | <span data-ttu-id="c4901-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c4901-120">Type</span></span>        | <span data-ttu-id="c4901-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c4901-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c4901-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4901-122">Authorization</span></span> | <span data-ttu-id="c4901-123">string</span><span class="sxs-lookup"><span data-stu-id="c4901-123">string</span></span> | <span data-ttu-id="c4901-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4901-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4901-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4901-126">Request body</span></span>
<span data-ttu-id="c4901-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4901-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="c4901-128">В следующей таблице приведены свойства, которые можно указать при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="c4901-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="c4901-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4901-129">Property</span></span>     | <span data-ttu-id="c4901-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c4901-130">Type</span></span>        | <span data-ttu-id="c4901-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c4901-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="c4901-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="c4901-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="c4901-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="c4901-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="c4901-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4901-134">Response</span></span>
<span data-ttu-id="c4901-135">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4901-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4901-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c4901-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4901-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4901-137">Request</span></span>
<span data-ttu-id="c4901-138">В тексте запроса добавьте представление объекта [программы](../resources/program.md) , который необходимо изменить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4901-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="c4901-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4901-139">Response</span></span>
><span data-ttu-id="c4901-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4901-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c4901-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c4901-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c4901-143">C#</span><span class="sxs-lookup"><span data-stu-id="c4901-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4901-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4901-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_program-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c4901-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c4901-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_program-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="c4901-146">См. также</span><span class="sxs-lookup"><span data-stu-id="c4901-146">See also</span></span>

| <span data-ttu-id="c4901-147">Метод</span><span class="sxs-lookup"><span data-stu-id="c4901-147">Method</span></span>           | <span data-ttu-id="c4901-148">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4901-148">Return Type</span></span>    |<span data-ttu-id="c4901-149">Описание</span><span class="sxs-lookup"><span data-stu-id="c4901-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4901-150">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="c4901-150">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="c4901-151">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="c4901-151">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="c4901-152">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="c4901-152">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="c4901-153">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c4901-153">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="c4901-154">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="c4901-154">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="c4901-155">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="c4901-155">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
