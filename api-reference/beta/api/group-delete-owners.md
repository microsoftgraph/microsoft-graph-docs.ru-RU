---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
ms.openlocfilehash: af45706e6f42f3442e28dd8a04fe6863f957a6fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843360"
---
# <a name="remove-owner"></a><span data-ttu-id="0f84d-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="0f84d-103">Remove owner</span></span>

> <span data-ttu-id="0f84d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f84d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f84d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f84d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f84d-106">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="0f84d-106">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f84d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f84d-107">Permissions</span></span>
<span data-ttu-id="0f84d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f84d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f84d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f84d-110">Permission type</span></span>      | <span data-ttu-id="0f84d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f84d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f84d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f84d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0f84d-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0f84d-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0f84d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f84d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f84d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f84d-115">Not supported.</span></span>    |
|<span data-ttu-id="0f84d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f84d-116">Application</span></span> | <span data-ttu-id="0f84d-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f84d-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f84d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f84d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0f84d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f84d-119">Request headers</span></span>
| <span data-ttu-id="0f84d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0f84d-120">Name</span></span>       | <span data-ttu-id="0f84d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0f84d-121">Type</span></span> | <span data-ttu-id="0f84d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0f84d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f84d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f84d-123">Authorization</span></span>  | <span data-ttu-id="0f84d-124">string</span><span class="sxs-lookup"><span data-stu-id="0f84d-124">string</span></span>  | <span data-ttu-id="0f84d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f84d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f84d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f84d-127">Request body</span></span>
<span data-ttu-id="0f84d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f84d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f84d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f84d-129">Response</span></span>
<span data-ttu-id="0f84d-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0f84d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f84d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0f84d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0f84d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f84d-133">Request</span></span>
<span data-ttu-id="0f84d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f84d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="0f84d-135">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="0f84d-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="0f84d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f84d-136">Response</span></span>
<span data-ttu-id="0f84d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f84d-137">The following is an example of the response.</span></span>
><span data-ttu-id="0f84d-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="0f84d-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0f84d-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f84d-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
