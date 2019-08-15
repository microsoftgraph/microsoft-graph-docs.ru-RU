---
title: Программа обновления
description: В функции проверки доступа Azure AD обновите существующий объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c1f50f81d4c87283ce686da5626b5482055ec5fd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412497"
---
# <a name="update-program"></a><span data-ttu-id="8ace3-103">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="8ace3-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ace3-104">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="8ace3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ace3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ace3-105">Permissions</span></span>
<span data-ttu-id="8ace3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ace3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ace3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ace3-108">Permission type</span></span>                        | <span data-ttu-id="8ace3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ace3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ace3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ace3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ace3-111">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ace3-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="8ace3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ace3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ace3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ace3-113">Not supported.</span></span> |
|<span data-ttu-id="8ace3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ace3-114">Application</span></span>                            | <span data-ttu-id="8ace3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ace3-115">Not supported.</span></span> |

<span data-ttu-id="8ace3-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им обновлять программу.</span><span class="sxs-lookup"><span data-stu-id="8ace3-116">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="8ace3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ace3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="8ace3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ace3-118">Request headers</span></span>
| <span data-ttu-id="8ace3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8ace3-119">Name</span></span>         | <span data-ttu-id="8ace3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8ace3-120">Type</span></span>        | <span data-ttu-id="8ace3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ace3-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8ace3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ace3-122">Authorization</span></span> | <span data-ttu-id="8ace3-123">string</span><span class="sxs-lookup"><span data-stu-id="8ace3-123">string</span></span> | <span data-ttu-id="8ace3-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ace3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ace3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ace3-126">Request body</span></span>
<span data-ttu-id="8ace3-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ace3-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="8ace3-128">В следующей таблице приведены свойства, которые можно указать при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="8ace3-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="8ace3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ace3-129">Property</span></span>     | <span data-ttu-id="8ace3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8ace3-130">Type</span></span>        | <span data-ttu-id="8ace3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8ace3-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="8ace3-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="8ace3-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="8ace3-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="8ace3-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="8ace3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ace3-134">Response</span></span>
<span data-ttu-id="8ace3-135">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ace3-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ace3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8ace3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ace3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ace3-137">Request</span></span>
<span data-ttu-id="8ace3-138">В тексте запроса добавьте представление объекта [программы](../resources/program.md) , который необходимо изменить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ace3-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ace3-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ace3-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ace3-140">C#</span><span class="sxs-lookup"><span data-stu-id="8ace3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ace3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ace3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ace3-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8ace3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ace3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ace3-143">Response</span></span>
><span data-ttu-id="8ace3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ace3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8ace3-146">См. также</span><span class="sxs-lookup"><span data-stu-id="8ace3-146">See also</span></span>

| <span data-ttu-id="8ace3-147">Метод</span><span class="sxs-lookup"><span data-stu-id="8ace3-147">Method</span></span>           | <span data-ttu-id="8ace3-148">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ace3-148">Return Type</span></span>    |<span data-ttu-id="8ace3-149">Описание</span><span class="sxs-lookup"><span data-stu-id="8ace3-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ace3-150">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="8ace3-150">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="8ace3-151">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8ace3-151">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="8ace3-152">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="8ace3-152">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8ace3-153">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="8ace3-153">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="8ace3-154">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="8ace3-154">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="8ace3-155">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="8ace3-155">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
