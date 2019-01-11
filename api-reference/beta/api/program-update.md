---
title: Обновите программу
description: Доступ к функции проверки в Azure AD "," Обновление существующий объект программы.
localization_priority: Normal
ms.openlocfilehash: a9abe10a2a672984d14f1da821b7ae6244cbdf39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840336"
---
# <a name="update-program"></a><span data-ttu-id="4bdec-103">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="4bdec-103">Update program</span></span>

> <span data-ttu-id="4bdec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4bdec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bdec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bdec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bdec-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4bdec-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bdec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bdec-107">Permissions</span></span>
<span data-ttu-id="4bdec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bdec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bdec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bdec-110">Permission type</span></span>                        | <span data-ttu-id="4bdec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bdec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bdec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bdec-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bdec-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="4bdec-113"></span></span>  <span data-ttu-id="4bdec-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать обновления программы.</span><span class="sxs-lookup"><span data-stu-id="4bdec-114">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="4bdec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bdec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bdec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bdec-116">Not supported.</span></span> |
|<span data-ttu-id="4bdec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bdec-117">Application</span></span>                            | <span data-ttu-id="4bdec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bdec-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bdec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bdec-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="4bdec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bdec-120">Request headers</span></span>
| <span data-ttu-id="4bdec-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4bdec-121">Name</span></span>         | <span data-ttu-id="4bdec-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4bdec-122">Type</span></span>        | <span data-ttu-id="4bdec-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4bdec-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4bdec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bdec-124">Authorization</span></span> | <span data-ttu-id="4bdec-125">string</span><span class="sxs-lookup"><span data-stu-id="4bdec-125">string</span></span> | <span data-ttu-id="4bdec-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="4bdec-126">Bearer \{token\}.</span></span> <span data-ttu-id="4bdec-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bdec-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bdec-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bdec-128">Request body</span></span>
<span data-ttu-id="4bdec-129">В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4bdec-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="4bdec-130">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="4bdec-130">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="4bdec-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bdec-131">Property</span></span>     | <span data-ttu-id="4bdec-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4bdec-132">Type</span></span>        | <span data-ttu-id="4bdec-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4bdec-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="4bdec-134">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="4bdec-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="4bdec-135">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="4bdec-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="4bdec-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bdec-136">Response</span></span>
<span data-ttu-id="4bdec-137">Успешно завершена, этот метод возвращает `204, Accepted` объект [программы](../resources/program.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4bdec-137">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bdec-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4bdec-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bdec-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bdec-139">Request</span></span>
<span data-ttu-id="4bdec-140">В тексте запроса укажите представление JSON параметров объекта [программа](../resources/program.md) для изменения.</span><span class="sxs-lookup"><span data-stu-id="4bdec-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="4bdec-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bdec-141">Response</span></span>
><span data-ttu-id="4bdec-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bdec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4bdec-144">См. также</span><span class="sxs-lookup"><span data-stu-id="4bdec-144">See also</span></span>

| <span data-ttu-id="4bdec-145">Метод</span><span class="sxs-lookup"><span data-stu-id="4bdec-145">Method</span></span>           | <span data-ttu-id="4bdec-146">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4bdec-146">Return Type</span></span>    |<span data-ttu-id="4bdec-147">Описание</span><span class="sxs-lookup"><span data-stu-id="4bdec-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bdec-148">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="4bdec-148">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4bdec-149">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4bdec-149">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4bdec-150">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="4bdec-150">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="4bdec-151">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="4bdec-151">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="4bdec-152">programControl</span><span class="sxs-lookup"><span data-stu-id="4bdec-152">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="4bdec-153">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="4bdec-153">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
