---
title: Добавление участника
description: С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7f5d0b2e806d366c862466e466dd6f0e449b2a2b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277674"
---
# <a name="add-member"></a><span data-ttu-id="4544f-103">Добавление члена</span><span class="sxs-lookup"><span data-stu-id="4544f-103">Add member</span></span>
<span data-ttu-id="4544f-104">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="4544f-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="4544f-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="4544f-105">You can add users or other groups.</span></span> <span data-ttu-id="4544f-106">Важно! В Группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="4544f-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="4544f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4544f-107">Permissions</span></span>
<span data-ttu-id="4544f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4544f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4544f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4544f-110">Permission type</span></span>      | <span data-ttu-id="4544f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4544f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4544f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4544f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4544f-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4544f-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4544f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4544f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4544f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4544f-115">Not supported.</span></span>    |
|<span data-ttu-id="4544f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4544f-116">Application</span></span> | <span data-ttu-id="4544f-117">Group.ReadWrite.All and Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4544f-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4544f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4544f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4544f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4544f-119">Request headers</span></span>
| <span data-ttu-id="4544f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4544f-120">Name</span></span>       | <span data-ttu-id="4544f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4544f-121">Type</span></span> | <span data-ttu-id="4544f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4544f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4544f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4544f-123">Authorization</span></span>  | <span data-ttu-id="4544f-124">string</span><span class="sxs-lookup"><span data-stu-id="4544f-124">string</span></span>  | <span data-ttu-id="4544f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4544f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4544f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4544f-127">Request body</span></span>
<span data-ttu-id="4544f-128">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4544f-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="4544f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4544f-129">Response</span></span>
<span data-ttu-id="4544f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4544f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4544f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4544f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4544f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4544f-133">Request</span></span>
<span data-ttu-id="4544f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4544f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="4544f-135">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4544f-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="4544f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4544f-136">Response</span></span>
<span data-ttu-id="4544f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4544f-137">The following is an example of the response.</span></span>
><span data-ttu-id="4544f-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4544f-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4544f-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4544f-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4544f-140">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="4544f-140">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4544f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4544f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4544f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4544f-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
