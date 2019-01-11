---
title: Удаление элемента
description: С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.
localization_priority: Normal
ms.openlocfilehash: 917e662158785111847d5d74821bfedbb61205dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864479"
---
# <a name="remove-member"></a><span data-ttu-id="16894-104">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="16894-104">Remove member</span></span>

> <span data-ttu-id="16894-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16894-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16894-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16894-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16894-p103">С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="16894-p103">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="16894-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16894-109">Permissions</span></span>
<span data-ttu-id="16894-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16894-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16894-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16894-112">Permission type</span></span>      | <span data-ttu-id="16894-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16894-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16894-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16894-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16894-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16894-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16894-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16894-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16894-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16894-117">Not supported.</span></span>    |
|<span data-ttu-id="16894-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16894-118">Application</span></span> | <span data-ttu-id="16894-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16894-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16894-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16894-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="16894-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16894-121">Request headers</span></span>
| <span data-ttu-id="16894-122">Имя</span><span class="sxs-lookup"><span data-stu-id="16894-122">Name</span></span>       | <span data-ttu-id="16894-123">Тип</span><span class="sxs-lookup"><span data-stu-id="16894-123">Type</span></span> | <span data-ttu-id="16894-124">Описание</span><span class="sxs-lookup"><span data-stu-id="16894-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16894-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16894-125">Authorization</span></span>  | <span data-ttu-id="16894-126">string</span><span class="sxs-lookup"><span data-stu-id="16894-126">string</span></span>  | <span data-ttu-id="16894-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16894-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16894-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16894-129">Request body</span></span>
<span data-ttu-id="16894-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16894-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16894-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="16894-131">Response</span></span>
<span data-ttu-id="16894-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="16894-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16894-134">Пример</span><span class="sxs-lookup"><span data-stu-id="16894-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16894-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="16894-135">Request</span></span>
<span data-ttu-id="16894-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16894-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="16894-137">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="16894-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="16894-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="16894-138">Response</span></span>
<span data-ttu-id="16894-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="16894-139">The following is an example of the response.</span></span>
><span data-ttu-id="16894-140">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="16894-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16894-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16894-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
