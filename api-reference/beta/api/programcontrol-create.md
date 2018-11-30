---
title: Создание programControl
description: В Azure AD доступа к функции проверки, создайте новый объект programControl.  Это связывает проверки доступа к программе.
ms.openlocfilehash: fa6a93b13391fd4b9e3c5816bb2a27259e730c0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080368"
---
# <a name="create-programcontrol"></a><span data-ttu-id="6701b-104">Создание programControl</span><span class="sxs-lookup"><span data-stu-id="6701b-104">Create programControl</span></span>

> <span data-ttu-id="6701b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6701b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6701b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6701b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6701b-107">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="6701b-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="6701b-108">Это связывает проверки доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="6701b-108">This links an access review to a program.</span></span>

<span data-ttu-id="6701b-109">До внесения этого запроса, вызывающий объект должен иметь ранее</span><span class="sxs-lookup"><span data-stu-id="6701b-109">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="6701b-110">[созданные программы](program-create.md) или [вернуть программу](program-list.md), иметь значение `programId` необходимо включить в запрос,</span><span class="sxs-lookup"><span data-stu-id="6701b-110">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="6701b-111">[создан проверки доступа](accessreview-create.md) или [получить обзор доступа](accessreview-get.md), иметь значение `controlId` необходимо включить в запрос, и</span><span class="sxs-lookup"><span data-stu-id="6701b-111">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="6701b-112">[получить список типов элементов управления программы](programcontroltype-list.md), иметь значение `controlTypeId` необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="6701b-112">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="6701b-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6701b-113">Permissions</span></span>
<span data-ttu-id="6701b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6701b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6701b-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6701b-116">Permission type</span></span>                        | <span data-ttu-id="6701b-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6701b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6701b-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6701b-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="6701b-119">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="6701b-119"></span></span>  <span data-ttu-id="6701b-120">Также должен быть выполнен вход пользователя в роль каталог, который позволяет использовать для создания programControl.</span><span class="sxs-lookup"><span data-stu-id="6701b-120">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="6701b-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6701b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6701b-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6701b-122">Not supported.</span></span> |
|<span data-ttu-id="6701b-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6701b-123">Application</span></span>                            | <span data-ttu-id="6701b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6701b-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6701b-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6701b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="6701b-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6701b-126">Request headers</span></span>
| <span data-ttu-id="6701b-127">Имя</span><span class="sxs-lookup"><span data-stu-id="6701b-127">Name</span></span>         | <span data-ttu-id="6701b-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6701b-128">Type</span></span>        | <span data-ttu-id="6701b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6701b-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6701b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6701b-130">Authorization</span></span> | <span data-ttu-id="6701b-131">string</span><span class="sxs-lookup"><span data-stu-id="6701b-131">string</span></span> | <span data-ttu-id="6701b-132">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="6701b-132">Bearer \{token\}.</span></span> <span data-ttu-id="6701b-133">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="6701b-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6701b-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6701b-134">Request body</span></span>
<span data-ttu-id="6701b-135">В тексте запроса укажите представление JSON объекта [programControl](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="6701b-135">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="6701b-136">Ниже приведены свойства, которые необходимы для создания элемента управления программы.</span><span class="sxs-lookup"><span data-stu-id="6701b-136">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="6701b-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="6701b-137">Property</span></span>     | <span data-ttu-id="6701b-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6701b-138">Type</span></span>        | <span data-ttu-id="6701b-139">Description</span><span class="sxs-lookup"><span data-stu-id="6701b-139">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="6701b-140">ProgramId программа этот элемент управления будет стать частью.</span><span class="sxs-lookup"><span data-stu-id="6701b-140">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="6701b-141">ControlId элемента управления, в частности идентификатор доступа просмотрите.</span><span class="sxs-lookup"><span data-stu-id="6701b-141">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="6701b-142">ProgramControlType определяет тип элемента управления, программа -, например дается обзор элемента управления, создание ссылок на доступ в качестве гостя.</span><span class="sxs-lookup"><span data-stu-id="6701b-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="6701b-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="6701b-143">Response</span></span>
<span data-ttu-id="6701b-144">Успешно завершена, этот метод возвращает `201, Created` код ответа и объект [programControl](../resources/programcontrol.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6701b-144">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="6701b-145">Пример</span><span class="sxs-lookup"><span data-stu-id="6701b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6701b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6701b-146">Request</span></span>
<span data-ttu-id="6701b-147">В тексте запроса укажите представление объекта [programControl](../resources/programcontrol.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="6701b-147">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="6701b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6701b-148">Response</span></span>
><span data-ttu-id="6701b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6701b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6701b-151">См. также</span><span class="sxs-lookup"><span data-stu-id="6701b-151">See also</span></span>

| <span data-ttu-id="6701b-152">Метод</span><span class="sxs-lookup"><span data-stu-id="6701b-152">Method</span></span>           | <span data-ttu-id="6701b-153">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6701b-153">Return Type</span></span>    |<span data-ttu-id="6701b-154">Описание</span><span class="sxs-lookup"><span data-stu-id="6701b-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6701b-155">Список programControlTypes</span><span class="sxs-lookup"><span data-stu-id="6701b-155">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="6701b-156">[programControlType](../resources/programcontroltype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6701b-156">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="6701b-157">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="6701b-157">List program control types.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
