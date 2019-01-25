---
title: Создание programControl
description: В Azure AD доступа к функции проверки, создайте новый объект programControl.  Это связывает проверки доступа к программе.
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511116"
---
# <a name="create-programcontrol"></a><span data-ttu-id="a534f-104">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="a534f-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a534f-105">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a534f-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="a534f-106">Это связывает проверки доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="a534f-106">This links an access review to a program.</span></span>

<span data-ttu-id="a534f-107">До внесения этого запроса, вызывающий объект должен иметь ранее</span><span class="sxs-lookup"><span data-stu-id="a534f-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="a534f-108">[созданные программы](program-create.md) или [вернуть программу](program-list.md), иметь значение `programId` необходимо включить в запрос,</span><span class="sxs-lookup"><span data-stu-id="a534f-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="a534f-109">[создан проверки доступа](accessreview-create.md) или [получить обзор доступа](accessreview-get.md), иметь значение `controlId` необходимо включить в запрос, и</span><span class="sxs-lookup"><span data-stu-id="a534f-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="a534f-110">[получить список типов элементов управления программы](programcontroltype-list.md), иметь значение `controlTypeId` необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="a534f-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="a534f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a534f-111">Permissions</span></span>
<span data-ttu-id="a534f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a534f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a534f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a534f-114">Permission type</span></span>                        | <span data-ttu-id="a534f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a534f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a534f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a534f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a534f-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="a534f-117"></span></span>  <span data-ttu-id="a534f-118">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания programControl.</span><span class="sxs-lookup"><span data-stu-id="a534f-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="a534f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a534f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a534f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a534f-120">Not supported.</span></span> |
|<span data-ttu-id="a534f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a534f-121">Application</span></span>                            | <span data-ttu-id="a534f-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a534f-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a534f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a534f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="a534f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a534f-124">Request headers</span></span>
| <span data-ttu-id="a534f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a534f-125">Name</span></span>         | <span data-ttu-id="a534f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a534f-126">Type</span></span>        | <span data-ttu-id="a534f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a534f-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a534f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a534f-128">Authorization</span></span> | <span data-ttu-id="a534f-129">string</span><span class="sxs-lookup"><span data-stu-id="a534f-129">string</span></span> | <span data-ttu-id="a534f-130">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="a534f-130">Bearer \{token\}.</span></span> <span data-ttu-id="a534f-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a534f-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a534f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a534f-132">Request body</span></span>
<span data-ttu-id="a534f-133">В тексте запроса укажите представление JSON объекта [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="a534f-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="a534f-134">Ниже приведены свойства, которые необходимы для создания элемента управления программы.</span><span class="sxs-lookup"><span data-stu-id="a534f-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="a534f-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="a534f-135">Property</span></span>     | <span data-ttu-id="a534f-136">Тип</span><span class="sxs-lookup"><span data-stu-id="a534f-136">Type</span></span>        | <span data-ttu-id="a534f-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a534f-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="a534f-138">ProgramId программа этот элемент управления будет стать частью.</span><span class="sxs-lookup"><span data-stu-id="a534f-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="a534f-139">ControlId элемента управления, в частности идентификатор доступа просмотрите.</span><span class="sxs-lookup"><span data-stu-id="a534f-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="a534f-140">ProgramControlType определяет тип элемента управления, программа -, например дается обзор элемента управления, создание ссылок на доступ в качестве гостя.</span><span class="sxs-lookup"><span data-stu-id="a534f-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="a534f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="a534f-141">Response</span></span>
<span data-ttu-id="a534f-142">Успешно завершена, этот метод возвращает `201, Created` код ответа и объект [programControl](../resources/programcontrol.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a534f-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="a534f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="a534f-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a534f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a534f-144">Request</span></span>
<span data-ttu-id="a534f-145">В тексте запроса укажите представление объекта [programControl](../resources/programcontrol.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="a534f-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a><span data-ttu-id="a534f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a534f-146">Response</span></span>
><span data-ttu-id="a534f-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a534f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a><span data-ttu-id="a534f-149">См. также</span><span class="sxs-lookup"><span data-stu-id="a534f-149">See also</span></span>

| <span data-ttu-id="a534f-150">Метод</span><span class="sxs-lookup"><span data-stu-id="a534f-150">Method</span></span>           | <span data-ttu-id="a534f-151">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a534f-151">Return Type</span></span>    |<span data-ttu-id="a534f-152">Описание</span><span class="sxs-lookup"><span data-stu-id="a534f-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a534f-153">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="a534f-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="a534f-154">[programControlType](../resources/programcontroltype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a534f-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="a534f-155">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="a534f-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
