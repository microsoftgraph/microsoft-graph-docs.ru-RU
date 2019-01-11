---
title: Создание программы
description: В Azure AD доступа к функции проверки, создайте новый объект.
localization_priority: Normal
ms.openlocfilehash: b982242bbdddb9769d64c9757d9041fddc215d53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844018"
---
# <a name="create-program"></a><span data-ttu-id="be04d-103">Создание программы</span><span class="sxs-lookup"><span data-stu-id="be04d-103">Create program</span></span>

> <span data-ttu-id="be04d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be04d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be04d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be04d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be04d-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте [новый объект](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="be04d-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be04d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be04d-107">Permissions</span></span>
<span data-ttu-id="be04d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be04d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be04d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be04d-110">Permission type</span></span>                        | <span data-ttu-id="be04d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be04d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="be04d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be04d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="be04d-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="be04d-113"></span></span>  <span data-ttu-id="be04d-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания программы.</span><span class="sxs-lookup"><span data-stu-id="be04d-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="be04d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be04d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be04d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be04d-116">Not supported.</span></span> |
|<span data-ttu-id="be04d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be04d-117">Application</span></span>                            | <span data-ttu-id="be04d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be04d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be04d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be04d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="be04d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be04d-120">Request headers</span></span>
| <span data-ttu-id="be04d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="be04d-121">Name</span></span>         | <span data-ttu-id="be04d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="be04d-122">Type</span></span>        | <span data-ttu-id="be04d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="be04d-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="be04d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be04d-124">Authorization</span></span> | <span data-ttu-id="be04d-125">string</span><span class="sxs-lookup"><span data-stu-id="be04d-125">string</span></span> | <span data-ttu-id="be04d-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="be04d-126">Bearer \{token\}.</span></span> <span data-ttu-id="be04d-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be04d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be04d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be04d-128">Request body</span></span>
<span data-ttu-id="be04d-129">В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="be04d-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="be04d-130">Ниже приведены свойства, которые необходимы для создания программы.</span><span class="sxs-lookup"><span data-stu-id="be04d-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="be04d-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="be04d-131">Property</span></span>     | <span data-ttu-id="be04d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="be04d-132">Type</span></span>        | <span data-ttu-id="be04d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="be04d-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="be04d-134">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="be04d-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="be04d-135">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="be04d-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="be04d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="be04d-136">Response</span></span>
<span data-ttu-id="be04d-137">Успешно завершена, этот метод возвращает `201, Created` объект [программы](../resources/program.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be04d-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be04d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="be04d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be04d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="be04d-139">Request</span></span>
<span data-ttu-id="be04d-140">В тексте запроса укажите представление объекта [программы](../resources/program.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="be04d-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="be04d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="be04d-141">Response</span></span>
><span data-ttu-id="be04d-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be04d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="be04d-144">См. также</span><span class="sxs-lookup"><span data-stu-id="be04d-144">See also</span></span>

| <span data-ttu-id="be04d-145">Метод</span><span class="sxs-lookup"><span data-stu-id="be04d-145">Method</span></span>           | <span data-ttu-id="be04d-146">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be04d-146">Return Type</span></span>    |<span data-ttu-id="be04d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="be04d-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be04d-148">Список программ</span><span class="sxs-lookup"><span data-stu-id="be04d-148">List programs</span></span>](program-list.md) | <span data-ttu-id="be04d-149">[программа](../resources/program.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="be04d-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="be04d-150">Получите коллекцию всех программ.</span><span class="sxs-lookup"><span data-stu-id="be04d-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="be04d-151">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="be04d-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="be04d-152">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="be04d-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="be04d-153">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="be04d-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="be04d-154">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="be04d-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="be04d-155">Программа</span><span class="sxs-lookup"><span data-stu-id="be04d-155">program</span></span>](../resources/program.md)| <span data-ttu-id="be04d-156">Обновите программу.</span><span class="sxs-lookup"><span data-stu-id="be04d-156">Update a program.</span></span>|
|[<span data-ttu-id="be04d-157">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="be04d-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="be04d-158">programControl</span><span class="sxs-lookup"><span data-stu-id="be04d-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="be04d-159">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="be04d-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
