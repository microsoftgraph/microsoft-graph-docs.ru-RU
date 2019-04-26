---
title: Обновление outlooktaskfolder
description: Обновление свойств, доступных для записи, папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9b7727ce554e5dccb24dae78e73d4692330691dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337915"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="418fc-103">Обновление outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="418fc-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418fc-104">Обновление свойств, доступных для записи, папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="418fc-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="418fc-105">Вы не можете изменить значение свойства **Name** папки задач по умолчанию, "задачи".</span><span class="sxs-lookup"><span data-stu-id="418fc-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="418fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="418fc-106">Permissions</span></span>
<span data-ttu-id="418fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="418fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="418fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="418fc-109">Permission type</span></span>      | <span data-ttu-id="418fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="418fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="418fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="418fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="418fc-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="418fc-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="418fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="418fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="418fc-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="418fc-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="418fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="418fc-115">Application</span></span> | <span data-ttu-id="418fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="418fc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="418fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="418fc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="418fc-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="418fc-118">Optional request headers</span></span>
| <span data-ttu-id="418fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="418fc-119">Name</span></span>       | <span data-ttu-id="418fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="418fc-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="418fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="418fc-121">Authorization</span></span>  | <span data-ttu-id="418fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="418fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="418fc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="418fc-124">Request body</span></span>
<span data-ttu-id="418fc-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="418fc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="418fc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="418fc-128">Property</span></span>     | <span data-ttu-id="418fc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="418fc-129">Type</span></span>   |<span data-ttu-id="418fc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="418fc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="418fc-131">name</span><span class="sxs-lookup"><span data-stu-id="418fc-131">name</span></span>|<span data-ttu-id="418fc-132">String</span><span class="sxs-lookup"><span data-stu-id="418fc-132">String</span></span>|<span data-ttu-id="418fc-133">Имя папки задач.</span><span class="sxs-lookup"><span data-stu-id="418fc-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="418fc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="418fc-134">Response</span></span>

<span data-ttu-id="418fc-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="418fc-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="418fc-136">Пример</span><span class="sxs-lookup"><span data-stu-id="418fc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="418fc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="418fc-137">Request</span></span>
<span data-ttu-id="418fc-138">В следующем примере показано изменение имени указанной папки задач на `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="418fc-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="418fc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="418fc-139">Response</span></span>
<span data-ttu-id="418fc-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="418fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
