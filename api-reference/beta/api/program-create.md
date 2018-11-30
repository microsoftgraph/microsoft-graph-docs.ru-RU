---
title: Создание программы
description: В Azure AD доступа к функции проверки, создайте новый объект.
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080820"
---
# <a name="create-program"></a><span data-ttu-id="c4b52-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="c4b52-103">Create program</span></span>

> <span data-ttu-id="c4b52-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4b52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4b52-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4b52-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте [новый объект](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="c4b52-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4b52-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4b52-107">Permissions</span></span>
<span data-ttu-id="c4b52-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4b52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b52-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4b52-110">Permission type</span></span>                        | <span data-ttu-id="c4b52-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4b52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4b52-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4b52-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4b52-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="c4b52-113"></span></span>  <span data-ttu-id="c4b52-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания программы.</span><span class="sxs-lookup"><span data-stu-id="c4b52-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="c4b52-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4b52-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4b52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b52-116">Not supported.</span></span> |
|<span data-ttu-id="c4b52-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4b52-117">Application</span></span>                            | <span data-ttu-id="c4b52-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b52-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4b52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4b52-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="c4b52-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4b52-120">Request headers</span></span>
| <span data-ttu-id="c4b52-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c4b52-121">Name</span></span>         | <span data-ttu-id="c4b52-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c4b52-122">Type</span></span>        | <span data-ttu-id="c4b52-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c4b52-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c4b52-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4b52-124">Authorization</span></span> | <span data-ttu-id="c4b52-125">string</span><span class="sxs-lookup"><span data-stu-id="c4b52-125">string</span></span> | <span data-ttu-id="c4b52-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="c4b52-126">Bearer \{token\}.</span></span> <span data-ttu-id="c4b52-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c4b52-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4b52-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4b52-128">Request body</span></span>
<span data-ttu-id="c4b52-129">В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="c4b52-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="c4b52-130">Ниже приведены свойства, которые необходимы для создания программы.</span><span class="sxs-lookup"><span data-stu-id="c4b52-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="c4b52-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4b52-131">Property</span></span>     | <span data-ttu-id="c4b52-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c4b52-132">Type</span></span>        | <span data-ttu-id="c4b52-133">Description</span><span class="sxs-lookup"><span data-stu-id="c4b52-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="c4b52-134">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="c4b52-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="c4b52-135">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="c4b52-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="c4b52-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4b52-136">Response</span></span>
<span data-ttu-id="c4b52-137">Успешно завершена, этот метод возвращает `201, Created` объект [программы](../resources/program.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c4b52-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4b52-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c4b52-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4b52-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4b52-139">Request</span></span>
<span data-ttu-id="c4b52-140">В тексте запроса укажите представление объекта [программы](../resources/program.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="c4b52-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c4b52-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4b52-141">Response</span></span>
><span data-ttu-id="c4b52-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4b52-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c4b52-144">См. также</span><span class="sxs-lookup"><span data-stu-id="c4b52-144">See also</span></span>

| <span data-ttu-id="c4b52-145">Метод</span><span class="sxs-lookup"><span data-stu-id="c4b52-145">Method</span></span>           | <span data-ttu-id="c4b52-146">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4b52-146">Return Type</span></span>    |<span data-ttu-id="c4b52-147">Описание</span><span class="sxs-lookup"><span data-stu-id="c4b52-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4b52-148">Список программ</span><span class="sxs-lookup"><span data-stu-id="c4b52-148">List programs</span></span>](program-list.md) | <span data-ttu-id="c4b52-149">[программа](../resources/program.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="c4b52-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="c4b52-150">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="c4b52-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="c4b52-151">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="c4b52-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="c4b52-152">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c4b52-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="c4b52-153">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="c4b52-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="c4b52-154">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="c4b52-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="c4b52-155">Программа</span><span class="sxs-lookup"><span data-stu-id="c4b52-155">program</span></span>](../resources/program.md)| <span data-ttu-id="c4b52-156">Обновите программу.</span><span class="sxs-lookup"><span data-stu-id="c4b52-156">Update a program.</span></span>|
|[<span data-ttu-id="c4b52-157">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="c4b52-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="c4b52-158">programControl</span><span class="sxs-lookup"><span data-stu-id="c4b52-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="c4b52-159">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="c4b52-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
