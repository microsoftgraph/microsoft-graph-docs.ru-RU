---
title: Обновление outlooktaskfolder
description: Обновление для записи свойств папки задач Outlook.
ms.openlocfilehash: 8b02f3b8eea104ba0a0cfaa3fddaf286fa41f389
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081692"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="e240d-103">Обновление outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="e240d-103">Update outlooktaskfolder</span></span>

> <span data-ttu-id="e240d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e240d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e240d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e240d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e240d-106">Обновление для записи свойств папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="e240d-106">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="e240d-107">Невозможно изменить значение свойства **имя** папки задач по умолчанию, «Задачи».</span><span class="sxs-lookup"><span data-stu-id="e240d-107">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="e240d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e240d-108">Permissions</span></span>
<span data-ttu-id="e240d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e240d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e240d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e240d-111">Permission type</span></span>      | <span data-ttu-id="e240d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e240d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e240d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e240d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e240d-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e240d-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e240d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e240d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e240d-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e240d-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="e240d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e240d-117">Application</span></span> | <span data-ttu-id="e240d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e240d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e240d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e240d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e240d-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e240d-120">Optional request headers</span></span>
| <span data-ttu-id="e240d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e240d-121">Name</span></span>       | <span data-ttu-id="e240d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e240d-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e240d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e240d-123">Authorization</span></span>  | <span data-ttu-id="e240d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e240d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e240d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e240d-126">Request body</span></span>
<span data-ttu-id="e240d-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e240d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e240d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e240d-130">Property</span></span>     | <span data-ttu-id="e240d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e240d-131">Type</span></span>   |<span data-ttu-id="e240d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e240d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e240d-133">name</span><span class="sxs-lookup"><span data-stu-id="e240d-133">name</span></span>|<span data-ttu-id="e240d-134">String</span><span class="sxs-lookup"><span data-stu-id="e240d-134">String</span></span>|<span data-ttu-id="e240d-135">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="e240d-135">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e240d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e240d-136">Response</span></span>

<span data-ttu-id="e240d-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [outlookTaskFolder](../resources/outlooktaskfolder.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e240d-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e240d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e240d-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e240d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e240d-139">Request</span></span>
<span data-ttu-id="e240d-140">В следующем примере изменяется имя папки указанной задачи для `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="e240d-140">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPWAAA=')
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="e240d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e240d-141">Response</span></span>
<span data-ttu-id="e240d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e240d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->