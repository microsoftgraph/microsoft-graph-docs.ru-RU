---
title: Обновление outlooktaskfolder
description: Обновление для записи свойств папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 83b75fb2588f58480e51e4e548bfd5d05b7f941b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530162"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="39ed2-103">Обновление outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="39ed2-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ed2-104">Обновление для записи свойств папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="39ed2-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="39ed2-105">Невозможно изменить значение свойства **имя** папки задач по умолчанию, «Задачи».</span><span class="sxs-lookup"><span data-stu-id="39ed2-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="39ed2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39ed2-106">Permissions</span></span>
<span data-ttu-id="39ed2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39ed2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39ed2-109">Permission type</span></span>      | <span data-ttu-id="39ed2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39ed2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39ed2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39ed2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39ed2-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39ed2-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="39ed2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39ed2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39ed2-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39ed2-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="39ed2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39ed2-115">Application</span></span> | <span data-ttu-id="39ed2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ed2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39ed2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39ed2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="39ed2-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39ed2-118">Optional request headers</span></span>
| <span data-ttu-id="39ed2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39ed2-119">Name</span></span>       | <span data-ttu-id="39ed2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39ed2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="39ed2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39ed2-121">Authorization</span></span>  | <span data-ttu-id="39ed2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ed2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39ed2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39ed2-124">Request body</span></span>
<span data-ttu-id="39ed2-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="39ed2-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="39ed2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="39ed2-128">Property</span></span>     | <span data-ttu-id="39ed2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="39ed2-129">Type</span></span>   |<span data-ttu-id="39ed2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="39ed2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ed2-131">name</span><span class="sxs-lookup"><span data-stu-id="39ed2-131">name</span></span>|<span data-ttu-id="39ed2-132">String</span><span class="sxs-lookup"><span data-stu-id="39ed2-132">String</span></span>|<span data-ttu-id="39ed2-133">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="39ed2-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="39ed2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="39ed2-134">Response</span></span>

<span data-ttu-id="39ed2-135">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [outlookTaskFolder](../resources/outlooktaskfolder.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="39ed2-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39ed2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="39ed2-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39ed2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="39ed2-137">Request</span></span>
<span data-ttu-id="39ed2-138">В следующем примере изменяется имя папки указанной задачи для `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="39ed2-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
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
##### <a name="response"></a><span data-ttu-id="39ed2-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="39ed2-139">Response</span></span>
<span data-ttu-id="39ed2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="39ed2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
