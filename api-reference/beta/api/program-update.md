---
title: Обновите программу
description: Доступ к функции проверки в Azure AD "," Обновление существующий объект программы.
ms.openlocfilehash: e3d8ca75683a076f156e359431204517b60e7c6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080167"
---
# <a name="update-program"></a><span data-ttu-id="a18f4-103">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="a18f4-103">Update program</span></span>

> <span data-ttu-id="a18f4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a18f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a18f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a18f4-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="a18f4-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a18f4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a18f4-107">Permissions</span></span>
<span data-ttu-id="a18f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a18f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a18f4-110">Permission type</span></span>                        | <span data-ttu-id="a18f4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a18f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a18f4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a18f4-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a18f4-113"></span></span>  <span data-ttu-id="a18f4-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать обновления программы.</span><span class="sxs-lookup"><span data-stu-id="a18f4-114">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="a18f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a18f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18f4-116">Not supported.</span></span> |
|<span data-ttu-id="a18f4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a18f4-117">Application</span></span>                            | <span data-ttu-id="a18f4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18f4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a18f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a18f4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="a18f4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a18f4-120">Request headers</span></span>
| <span data-ttu-id="a18f4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a18f4-121">Name</span></span>         | <span data-ttu-id="a18f4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a18f4-122">Type</span></span>        | <span data-ttu-id="a18f4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a18f4-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a18f4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a18f4-124">Authorization</span></span> | <span data-ttu-id="a18f4-125">string</span><span class="sxs-lookup"><span data-stu-id="a18f4-125">string</span></span> | <span data-ttu-id="a18f4-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="a18f4-126">Bearer \{token\}.</span></span> <span data-ttu-id="a18f4-127">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="a18f4-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a18f4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a18f4-128">Request body</span></span>
<span data-ttu-id="a18f4-129">В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="a18f4-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="a18f4-130">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="a18f4-130">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="a18f4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a18f4-131">Property</span></span>     | <span data-ttu-id="a18f4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a18f4-132">Type</span></span>        | <span data-ttu-id="a18f4-133">Description</span><span class="sxs-lookup"><span data-stu-id="a18f4-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="a18f4-134">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="a18f4-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="a18f4-135">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="a18f4-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="a18f4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a18f4-136">Response</span></span>
<span data-ttu-id="a18f4-137">Успешно завершена, этот метод возвращает `204, Accepted` объект [программы](../resources/program.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a18f4-137">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18f4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a18f4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a18f4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a18f4-139">Request</span></span>
<span data-ttu-id="a18f4-140">В тексте запроса укажите представление JSON параметров объекта [программа](../resources/program.md) для изменения.</span><span class="sxs-lookup"><span data-stu-id="a18f4-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="a18f4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18f4-141">Response</span></span>
><span data-ttu-id="a18f4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a18f4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a18f4-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a18f4-144">See also</span></span>

| <span data-ttu-id="a18f4-145">Метод</span><span class="sxs-lookup"><span data-stu-id="a18f4-145">Method</span></span>           | <span data-ttu-id="a18f4-146">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a18f4-146">Return Type</span></span>    |<span data-ttu-id="a18f4-147">Описание</span><span class="sxs-lookup"><span data-stu-id="a18f4-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a18f4-148">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="a18f4-148">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="a18f4-149">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a18f4-149">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="a18f4-150">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="a18f4-150">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="a18f4-151">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="a18f4-151">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="a18f4-152">programControl</span><span class="sxs-lookup"><span data-stu-id="a18f4-152">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="a18f4-153">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="a18f4-153">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
