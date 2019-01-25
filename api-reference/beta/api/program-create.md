---
title: Создание программы
description: В Azure AD доступа к функции проверки, создайте новый объект.
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521301"
---
# <a name="create-program"></a><span data-ttu-id="ce0d3-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="ce0d3-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce0d3-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте [новый объект](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="ce0d3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce0d3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce0d3-105">Permissions</span></span>
<span data-ttu-id="ce0d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce0d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce0d3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce0d3-108">Permission type</span></span>                        | <span data-ttu-id="ce0d3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce0d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce0d3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce0d3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce0d3-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-111"></span></span>  <span data-ttu-id="ce0d3-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания программы.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-112">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="ce0d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce0d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-114">Not supported.</span></span> |
|<span data-ttu-id="ce0d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce0d3-115">Application</span></span>                            | <span data-ttu-id="ce0d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce0d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce0d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="ce0d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce0d3-118">Request headers</span></span>
| <span data-ttu-id="ce0d3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ce0d3-119">Name</span></span>         | <span data-ttu-id="ce0d3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ce0d3-120">Type</span></span>        | <span data-ttu-id="ce0d3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0d3-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ce0d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce0d3-122">Authorization</span></span> | <span data-ttu-id="ce0d3-123">string</span><span class="sxs-lookup"><span data-stu-id="ce0d3-123">string</span></span> | <span data-ttu-id="ce0d3-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="ce0d3-124">Bearer \{token\}.</span></span> <span data-ttu-id="ce0d3-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce0d3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce0d3-126">Request body</span></span>
<span data-ttu-id="ce0d3-127">В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="ce0d3-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="ce0d3-128">Ниже приведены свойства, которые необходимы для создания программы.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="ce0d3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce0d3-129">Property</span></span>     | <span data-ttu-id="ce0d3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ce0d3-130">Type</span></span>        | <span data-ttu-id="ce0d3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0d3-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="ce0d3-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="ce0d3-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="ce0d3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce0d3-134">Response</span></span>
<span data-ttu-id="ce0d3-135">Успешно завершена, этот метод возвращает `201, Created` объект [программы](../resources/program.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce0d3-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ce0d3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce0d3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce0d3-137">Request</span></span>
<span data-ttu-id="ce0d3-138">В тексте запроса укажите представление объекта [программы](../resources/program.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="ce0d3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce0d3-139">Response</span></span>
><span data-ttu-id="ce0d3-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ce0d3-142">См. также</span><span class="sxs-lookup"><span data-stu-id="ce0d3-142">See also</span></span>

| <span data-ttu-id="ce0d3-143">Метод</span><span class="sxs-lookup"><span data-stu-id="ce0d3-143">Method</span></span>           | <span data-ttu-id="ce0d3-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce0d3-144">Return Type</span></span>    |<span data-ttu-id="ce0d3-145">Описание</span><span class="sxs-lookup"><span data-stu-id="ce0d3-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce0d3-146">Список программ</span><span class="sxs-lookup"><span data-stu-id="ce0d3-146">List programs</span></span>](program-list.md) | <span data-ttu-id="ce0d3-147">[программа](../resources/program.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="ce0d3-147">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="ce0d3-148">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-148">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="ce0d3-149">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="ce0d3-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="ce0d3-150">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ce0d3-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="ce0d3-151">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="ce0d3-152">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="ce0d3-152">Update program</span></span>](program-update.md) |  [<span data-ttu-id="ce0d3-153">Программа</span><span class="sxs-lookup"><span data-stu-id="ce0d3-153">program</span></span>](../resources/program.md)| <span data-ttu-id="ce0d3-154">Обновите программу.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-154">Update a program.</span></span>|
|[<span data-ttu-id="ce0d3-155">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="ce0d3-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="ce0d3-156">programControl</span><span class="sxs-lookup"><span data-stu-id="ce0d3-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="ce0d3-157">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="ce0d3-157">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
