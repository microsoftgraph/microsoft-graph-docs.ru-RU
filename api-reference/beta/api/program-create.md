---
title: Создание программы
description: В функции рецензирования Access Azure AD создайте объект программы.
localization_priority: Normal
ms.openlocfilehash: 7ba329924761b1f43d0fc0fff02c6578b3a64a72
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337223"
---
# <a name="create-program"></a><span data-ttu-id="90967-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="90967-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90967-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD создайте объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="90967-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90967-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90967-105">Permissions</span></span>
<span data-ttu-id="90967-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90967-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90967-108">Permission type</span></span>                        | <span data-ttu-id="90967-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90967-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="90967-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90967-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="90967-111">Програмконтрол. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="90967-111">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="90967-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90967-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90967-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90967-113">Not supported.</span></span> |
|<span data-ttu-id="90967-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90967-114">Application</span></span>                            | <span data-ttu-id="90967-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90967-115">Not supported.</span></span> |

<span data-ttu-id="90967-116">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="90967-116">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="90967-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90967-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="90967-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90967-118">Request headers</span></span>
| <span data-ttu-id="90967-119">Имя</span><span class="sxs-lookup"><span data-stu-id="90967-119">Name</span></span>         | <span data-ttu-id="90967-120">Тип</span><span class="sxs-lookup"><span data-stu-id="90967-120">Type</span></span>        | <span data-ttu-id="90967-121">Описание</span><span class="sxs-lookup"><span data-stu-id="90967-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="90967-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90967-122">Authorization</span></span> | <span data-ttu-id="90967-123">string</span><span class="sxs-lookup"><span data-stu-id="90967-123">string</span></span> | <span data-ttu-id="90967-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90967-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90967-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90967-126">Request body</span></span>
<span data-ttu-id="90967-127">В тексте запроса добавьте представление объекта [программы](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90967-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="90967-128">В следующей таблице приведены свойства, необходимые при создании программы.</span><span class="sxs-lookup"><span data-stu-id="90967-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="90967-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="90967-129">Property</span></span>     | <span data-ttu-id="90967-130">Тип</span><span class="sxs-lookup"><span data-stu-id="90967-130">Type</span></span>        | <span data-ttu-id="90967-131">Описание</span><span class="sxs-lookup"><span data-stu-id="90967-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="90967-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="90967-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="90967-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="90967-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="90967-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90967-134">Response</span></span>
<span data-ttu-id="90967-135">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [Program](../resources/program.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90967-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90967-136">Пример</span><span class="sxs-lookup"><span data-stu-id="90967-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90967-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="90967-137">Request</span></span>
<span data-ttu-id="90967-138">В тексте запроса добавьте представление объекта [Program](../resources/program.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90967-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="90967-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="90967-139">Response</span></span>
><span data-ttu-id="90967-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90967-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="90967-142">См. также</span><span class="sxs-lookup"><span data-stu-id="90967-142">See also</span></span>

| <span data-ttu-id="90967-143">Метод</span><span class="sxs-lookup"><span data-stu-id="90967-143">Method</span></span>           | <span data-ttu-id="90967-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90967-144">Return Type</span></span>    |<span data-ttu-id="90967-145">Описание</span><span class="sxs-lookup"><span data-stu-id="90967-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90967-146">Список программ</span><span class="sxs-lookup"><span data-stu-id="90967-146">List programs</span></span>](program-list.md) | <span data-ttu-id="90967-147">Коллекция [Program](../resources/program.md)</span><span class="sxs-lookup"><span data-stu-id="90967-147">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="90967-148">Получение коллекции всех программ.</span><span class="sxs-lookup"><span data-stu-id="90967-148">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="90967-149">Список Програмконтролс программы</span><span class="sxs-lookup"><span data-stu-id="90967-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="90967-150">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="90967-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="90967-151">Получение коллекции элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="90967-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="90967-152">Программа обновления</span><span class="sxs-lookup"><span data-stu-id="90967-152">Update program</span></span>](program-update.md) |  [<span data-ttu-id="90967-153">Программа</span><span class="sxs-lookup"><span data-stu-id="90967-153">program</span></span>](../resources/program.md)| <span data-ttu-id="90967-154">Обновление программы.</span><span class="sxs-lookup"><span data-stu-id="90967-154">Update a program.</span></span>|
|[<span data-ttu-id="90967-155">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="90967-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="90967-156">Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="90967-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="90967-157">Добавление Програмконтрол в программу.</span><span class="sxs-lookup"><span data-stu-id="90967-157">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
