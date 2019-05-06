---
title: Программа обновления
description: В функции проверки доступа Azure AD обновите существующий объект программы.
localization_priority: Normal
ms.openlocfilehash: ca668a84fc39601d94f71c1666b975f3b61a6802
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611168"
---
# <a name="update-program"></a><span data-ttu-id="7ff12-103">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="7ff12-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff12-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="7ff12-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ff12-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff12-105">Permissions</span></span>
<span data-ttu-id="7ff12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff12-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ff12-108">Permission type</span></span>                        | <span data-ttu-id="7ff12-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ff12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ff12-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ff12-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ff12-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff12-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="7ff12-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ff12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ff12-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff12-113">Not supported.</span></span> |
|<span data-ttu-id="7ff12-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ff12-114">Application</span></span>                            | <span data-ttu-id="7ff12-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ff12-115">Not supported.</span></span> |

<span data-ttu-id="7ff12-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им обновлять программу.</span><span class="sxs-lookup"><span data-stu-id="7ff12-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="7ff12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ff12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="7ff12-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ff12-118">Request headers</span></span>
| <span data-ttu-id="7ff12-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7ff12-119">Name</span></span>         | <span data-ttu-id="7ff12-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff12-120">Type</span></span>        | <span data-ttu-id="7ff12-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff12-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7ff12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff12-122">Authorization</span></span> | <span data-ttu-id="7ff12-123">string</span><span class="sxs-lookup"><span data-stu-id="7ff12-123">string</span></span> | <span data-ttu-id="7ff12-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ff12-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ff12-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ff12-126">Request body</span></span>
<span data-ttu-id="7ff12-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff12-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="7ff12-128">В следующей таблице приведены свойства, которые можно указать при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="7ff12-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="7ff12-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ff12-129">Property</span></span>     | <span data-ttu-id="7ff12-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff12-130">Type</span></span>        | <span data-ttu-id="7ff12-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff12-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="7ff12-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="7ff12-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="7ff12-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="7ff12-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="7ff12-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff12-134">Response</span></span>
<span data-ttu-id="7ff12-135">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ff12-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ff12-136">Пример</span><span class="sxs-lookup"><span data-stu-id="7ff12-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ff12-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ff12-137">Request</span></span>
<span data-ttu-id="7ff12-138">В тексте запроса добавьте представление объекта [программы](../resources/program.md) , который необходимо изменить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ff12-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="7ff12-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ff12-139">Response</span></span>
><span data-ttu-id="7ff12-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ff12-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7ff12-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7ff12-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7ff12-143">Языках</span><span class="sxs-lookup"><span data-stu-id="7ff12-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ff12-144">Язык</span><span class="sxs-lookup"><span data-stu-id="7ff12-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_program-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="7ff12-145">См. также</span><span class="sxs-lookup"><span data-stu-id="7ff12-145">See also</span></span>

| <span data-ttu-id="7ff12-146">Метод</span><span class="sxs-lookup"><span data-stu-id="7ff12-146">Method</span></span>           | <span data-ttu-id="7ff12-147">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ff12-147">Return Type</span></span>    |<span data-ttu-id="7ff12-148">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff12-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ff12-149">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="7ff12-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="7ff12-150">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="7ff12-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="7ff12-151">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="7ff12-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="7ff12-152">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="7ff12-152">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="7ff12-153">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="7ff12-153">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="7ff12-154">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="7ff12-154">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
