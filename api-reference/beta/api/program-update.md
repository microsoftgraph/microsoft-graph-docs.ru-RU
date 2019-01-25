---
title: Обновите программу
description: Доступ к функции проверки в Azure AD "," Обновление существующий объект программы.
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529924"
---
# <a name="update-program"></a><span data-ttu-id="8278d-103">Обновите программу</span><span class="sxs-lookup"><span data-stu-id="8278d-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8278d-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD обновите существующий объект [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="8278d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8278d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8278d-105">Permissions</span></span>
<span data-ttu-id="8278d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8278d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8278d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8278d-108">Permission type</span></span>                        | <span data-ttu-id="8278d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8278d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8278d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8278d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8278d-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="8278d-111"></span></span>  <span data-ttu-id="8278d-112">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать обновления программы.</span><span class="sxs-lookup"><span data-stu-id="8278d-112">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="8278d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8278d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8278d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8278d-114">Not supported.</span></span> |
|<span data-ttu-id="8278d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8278d-115">Application</span></span>                            | <span data-ttu-id="8278d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8278d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8278d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8278d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="8278d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8278d-118">Request headers</span></span>
| <span data-ttu-id="8278d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8278d-119">Name</span></span>         | <span data-ttu-id="8278d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8278d-120">Type</span></span>        | <span data-ttu-id="8278d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8278d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8278d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8278d-122">Authorization</span></span> | <span data-ttu-id="8278d-123">string</span><span class="sxs-lookup"><span data-stu-id="8278d-123">string</span></span> | <span data-ttu-id="8278d-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="8278d-124">Bearer \{token\}.</span></span> <span data-ttu-id="8278d-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8278d-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8278d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8278d-126">Request body</span></span>
<span data-ttu-id="8278d-127">В тексте запроса укажите представление JSON объекта [программы](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="8278d-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="8278d-128">В следующей таблице показаны свойства, которые могут быть предоставлены при обновлении программы.</span><span class="sxs-lookup"><span data-stu-id="8278d-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="8278d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8278d-129">Property</span></span>     | <span data-ttu-id="8278d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8278d-130">Type</span></span>        | <span data-ttu-id="8278d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8278d-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="8278d-132">Имя программы.</span><span class="sxs-lookup"><span data-stu-id="8278d-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="8278d-133">Описание программы.</span><span class="sxs-lookup"><span data-stu-id="8278d-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="8278d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8278d-134">Response</span></span>
<span data-ttu-id="8278d-135">Успешно завершена, этот метод возвращает `204, Accepted` объект [программы](../resources/program.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8278d-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8278d-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8278d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8278d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8278d-137">Request</span></span>
<span data-ttu-id="8278d-138">В тексте запроса укажите представление JSON параметров объекта [программа](../resources/program.md) для изменения.</span><span class="sxs-lookup"><span data-stu-id="8278d-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8278d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8278d-139">Response</span></span>
><span data-ttu-id="8278d-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8278d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8278d-142">См. также</span><span class="sxs-lookup"><span data-stu-id="8278d-142">See also</span></span>

| <span data-ttu-id="8278d-143">Метод</span><span class="sxs-lookup"><span data-stu-id="8278d-143">Method</span></span>           | <span data-ttu-id="8278d-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8278d-144">Return Type</span></span>    |<span data-ttu-id="8278d-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8278d-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8278d-146">Список programControls программы</span><span class="sxs-lookup"><span data-stu-id="8278d-146">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="8278d-147">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8278d-147">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="8278d-148">Получите коллекцию элементов управления из программы.</span><span class="sxs-lookup"><span data-stu-id="8278d-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="8278d-149">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="8278d-149">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="8278d-150">programControl</span><span class="sxs-lookup"><span data-stu-id="8278d-150">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="8278d-151">Добавьте programControl программы.</span><span class="sxs-lookup"><span data-stu-id="8278d-151">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
