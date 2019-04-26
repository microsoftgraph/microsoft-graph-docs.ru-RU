---
title: Создание outlookTaskFolder
description: Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ad276f3b1ae55abd64302fa3c0620ecbe712e514
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332650"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="07532-103">Создание outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="07532-103">Create outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07532-104">Создайте папку задач в группе задач по умолчанию (`My Tasks`) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="07532-104">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="07532-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07532-105">Permissions</span></span>
<span data-ttu-id="07532-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07532-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07532-108">Permission type</span></span>      | <span data-ttu-id="07532-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07532-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07532-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07532-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07532-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07532-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="07532-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07532-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07532-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07532-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="07532-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07532-114">Application</span></span> | <span data-ttu-id="07532-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07532-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07532-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07532-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="request-headers"></a><span data-ttu-id="07532-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07532-117">Request headers</span></span>
| <span data-ttu-id="07532-118">Имя</span><span class="sxs-lookup"><span data-stu-id="07532-118">Name</span></span>       | <span data-ttu-id="07532-119">Описание</span><span class="sxs-lookup"><span data-stu-id="07532-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07532-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07532-120">Authorization</span></span>  | <span data-ttu-id="07532-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07532-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07532-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07532-123">Request body</span></span>
<span data-ttu-id="07532-124">В тексте запроса добавьте представление объекта [OutlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07532-124">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="07532-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="07532-125">Response</span></span>

<span data-ttu-id="07532-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07532-126">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07532-127">Пример</span><span class="sxs-lookup"><span data-stu-id="07532-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07532-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="07532-128">Request</span></span>
<span data-ttu-id="07532-129">В следующем примере создается папка Task с именем "добровольный" в группе задач`My Tasks`по умолчанию () почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="07532-129">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
<span data-ttu-id="07532-130">В тексте запроса добавьте представление объекта [OutlookTaskFolder](../resources/outlooktaskfolder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07532-130">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="07532-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="07532-131">Response</span></span>
<span data-ttu-id="07532-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07532-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
