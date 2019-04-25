---
title: Создание Програмконтрол
description: В средстве проверки доступа Azure AD создайте новый объект Програмконтрол.  При этом будет связана проверка доступа к программе.
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546441"
---
# <a name="create-programcontrol"></a><span data-ttu-id="b5a00-104">Создание Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="b5a00-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5a00-105">В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [програмконтрол](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="b5a00-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="b5a00-106">При этом будет связана проверка доступа к программе.</span><span class="sxs-lookup"><span data-stu-id="b5a00-106">This links an access review to a program.</span></span>

<span data-ttu-id="b5a00-107">Перед выполнением этого запроса вызывающий абонент должен был</span><span class="sxs-lookup"><span data-stu-id="b5a00-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="b5a00-108">[созданная программа](program-create.md) или [получена программа](program-list.md)со значением `programId` , включаемым в запрос.</span><span class="sxs-lookup"><span data-stu-id="b5a00-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="b5a00-109">[создана проверка доступа](accessreview-create.md) или [полученная проверка доступа](accessreview-get.md), для которой значение `controlId` должно быть включено в запрос, а</span><span class="sxs-lookup"><span data-stu-id="b5a00-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="b5a00-110">[получен список типов программного управления](programcontroltype-list.md), чтобы включить в запрос значение `controlTypeId` , которое необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="b5a00-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="b5a00-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5a00-111">Permissions</span></span>
<span data-ttu-id="b5a00-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5a00-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a00-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5a00-114">Permission type</span></span>                        | <span data-ttu-id="b5a00-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5a00-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5a00-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5a00-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5a00-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b5a00-117"></span></span>  <span data-ttu-id="b5a00-118">Пользователь, вошедшего в систему, также должен находиться в роли каталога, что позволяет им создавать Програмконтрол.</span><span class="sxs-lookup"><span data-stu-id="b5a00-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="b5a00-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5a00-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5a00-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5a00-120">Not supported.</span></span> |
|<span data-ttu-id="b5a00-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5a00-121">Application</span></span>                            | <span data-ttu-id="b5a00-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5a00-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5a00-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5a00-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="b5a00-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5a00-124">Request headers</span></span>
| <span data-ttu-id="b5a00-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b5a00-125">Name</span></span>         | <span data-ttu-id="b5a00-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b5a00-126">Type</span></span>        | <span data-ttu-id="b5a00-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b5a00-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b5a00-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5a00-128">Authorization</span></span> | <span data-ttu-id="b5a00-129">string</span><span class="sxs-lookup"><span data-stu-id="b5a00-129">string</span></span> | <span data-ttu-id="b5a00-p105">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5a00-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5a00-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5a00-132">Request body</span></span>
<span data-ttu-id="b5a00-133">В тексте запроса добавьте представление объекта [Програмконтрол](../resources/programcontrol.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5a00-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="b5a00-134">В следующей таблице приведены свойства, необходимые при создании программного элемента управления.</span><span class="sxs-lookup"><span data-stu-id="b5a00-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="b5a00-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5a00-135">Property</span></span>     | <span data-ttu-id="b5a00-136">Тип</span><span class="sxs-lookup"><span data-stu-id="b5a00-136">Type</span></span>        | <span data-ttu-id="b5a00-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b5a00-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="b5a00-138">Програмид программы, которая будет являться частью этого элемента управления.</span><span class="sxs-lookup"><span data-stu-id="b5a00-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="b5a00-139">ControlId элемента управления, в частности идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="b5a00-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="b5a00-140">Програмконтролтипе определяет тип элемента управления программы, например элемент управления, который связывается с проверками гостевого доступа.</span><span class="sxs-lookup"><span data-stu-id="b5a00-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="b5a00-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5a00-141">Response</span></span>
<span data-ttu-id="b5a00-142">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [програмконтрол](../resources/programcontrol.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5a00-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b5a00-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b5a00-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5a00-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5a00-144">Request</span></span>
<span data-ttu-id="b5a00-145">В тексте запроса добавьте представление объекта [програмконтрол](../resources/programcontrol.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5a00-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b5a00-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5a00-146">Response</span></span>
><span data-ttu-id="b5a00-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5a00-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b5a00-149">См. также</span><span class="sxs-lookup"><span data-stu-id="b5a00-149">See also</span></span>

| <span data-ttu-id="b5a00-150">Метод</span><span class="sxs-lookup"><span data-stu-id="b5a00-150">Method</span></span>           | <span data-ttu-id="b5a00-151">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5a00-151">Return Type</span></span>    |<span data-ttu-id="b5a00-152">Описание</span><span class="sxs-lookup"><span data-stu-id="b5a00-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5a00-153">Список Програмконтролтипес</span><span class="sxs-lookup"><span data-stu-id="b5a00-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="b5a00-154">Коллекция [програмконтролтипе](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="b5a00-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="b5a00-155">Список типов элементов управления программы.</span><span class="sxs-lookup"><span data-stu-id="b5a00-155">List program control types.</span></span> |


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
