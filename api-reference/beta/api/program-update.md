---
title: Программа обновления
description: В функции проверки доступа Azure AD обновите существующий объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 79c95007bc87c6a54eb3fce16ea20510d832c530
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123118"
---
# <a name="update-program"></a><span data-ttu-id="ec230-103">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="ec230-103">Update program</span></span>

<span data-ttu-id="ec230-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec230-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec230-105">В функции проверки [доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="ec230-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec230-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec230-106">Permissions</span></span>
<span data-ttu-id="ec230-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec230-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec230-109">Permission type</span></span>                        | <span data-ttu-id="ec230-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec230-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec230-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec230-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec230-112">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec230-112">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="ec230-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec230-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec230-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec230-114">Not supported.</span></span> |
|<span data-ttu-id="ec230-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec230-115">Application</span></span>                            | <span data-ttu-id="ec230-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec230-116">Not supported.</span></span> |

<span data-ttu-id="ec230-117">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им обновлять программу.</span><span class="sxs-lookup"><span data-stu-id="ec230-117">The signed in user must also be in a directory role that permits them to update a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="ec230-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec230-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="ec230-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec230-119">Request headers</span></span>
| <span data-ttu-id="ec230-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec230-120">Name</span></span>         | <span data-ttu-id="ec230-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ec230-121">Type</span></span>        | <span data-ttu-id="ec230-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ec230-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ec230-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec230-123">Authorization</span></span> | <span data-ttu-id="ec230-124">string</span><span class="sxs-lookup"><span data-stu-id="ec230-124">string</span></span> | <span data-ttu-id="ec230-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec230-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec230-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec230-127">Request body</span></span>
<span data-ttu-id="ec230-128">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec230-128">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="ec230-129">В следующей таблице приведены свойства, которые можно указать при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="ec230-129">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="ec230-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec230-130">Property</span></span>     | <span data-ttu-id="ec230-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec230-131">Type</span></span>        | <span data-ttu-id="ec230-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec230-132">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="ec230-133">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="ec230-133">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="ec230-134">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="ec230-134">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="ec230-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec230-135">Response</span></span>
<span data-ttu-id="ec230-136">В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec230-136">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec230-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ec230-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec230-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec230-138">Request</span></span>
<span data-ttu-id="ec230-139">В тексте запроса добавьте представление объекта [программы](../resources/program.md) , который необходимо изменить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec230-139">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>


# <a name="http"></a>[<span data-ttu-id="ec230-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec230-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ec230-141">C#</span><span class="sxs-lookup"><span data-stu-id="ec230-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec230-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec230-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec230-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec230-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ec230-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec230-144">Response</span></span>
><span data-ttu-id="ec230-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec230-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ec230-147">См. также</span><span class="sxs-lookup"><span data-stu-id="ec230-147">See also</span></span>

| <span data-ttu-id="ec230-148">Метод</span><span class="sxs-lookup"><span data-stu-id="ec230-148">Method</span></span>           | <span data-ttu-id="ec230-149">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec230-149">Return Type</span></span>    |<span data-ttu-id="ec230-150">Описание</span><span class="sxs-lookup"><span data-stu-id="ec230-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec230-151">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="ec230-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ec230-152">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ec230-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ec230-153">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="ec230-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ec230-154">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="ec230-154">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="ec230-155">програмконтрол</span><span class="sxs-lookup"><span data-stu-id="ec230-155">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="ec230-156">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="ec230-156">Add a programControl to a program.</span></span>|

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
