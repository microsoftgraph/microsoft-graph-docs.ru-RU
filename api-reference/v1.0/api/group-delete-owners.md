---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
ms.openlocfilehash: 7fe13b00d2e14bf69c1e3903f09d641d81f2dc0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821653"
---
# <a name="remove-owner"></a><span data-ttu-id="70867-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="70867-103">Remove owner</span></span>
<span data-ttu-id="70867-104">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="70867-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="70867-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70867-105">Permissions</span></span>
<span data-ttu-id="70867-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70867-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70867-108">Permission type</span></span>      | <span data-ttu-id="70867-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70867-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70867-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70867-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70867-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70867-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70867-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70867-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70867-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70867-113">Not supported.</span></span>    |
|<span data-ttu-id="70867-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70867-114">Application</span></span> | <span data-ttu-id="70867-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70867-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70867-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70867-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="70867-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70867-117">Request headers</span></span>
| <span data-ttu-id="70867-118">Имя</span><span class="sxs-lookup"><span data-stu-id="70867-118">Name</span></span>       | <span data-ttu-id="70867-119">Тип</span><span class="sxs-lookup"><span data-stu-id="70867-119">Type</span></span> | <span data-ttu-id="70867-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70867-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70867-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70867-121">Authorization</span></span>  | <span data-ttu-id="70867-122">string</span><span class="sxs-lookup"><span data-stu-id="70867-122">string</span></span>  | <span data-ttu-id="70867-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70867-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70867-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70867-125">Request body</span></span>
<span data-ttu-id="70867-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70867-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70867-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="70867-127">Response</span></span>
<span data-ttu-id="70867-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="70867-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70867-130">Пример</span><span class="sxs-lookup"><span data-stu-id="70867-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="70867-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="70867-131">Request</span></span>
<span data-ttu-id="70867-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70867-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="70867-133">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="70867-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="70867-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70867-134">Response</span></span>
<span data-ttu-id="70867-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="70867-135">The following is an example of the response.</span></span>
><span data-ttu-id="70867-136">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="70867-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="70867-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70867-137">All the properties will be returned from an actual call.</span></span>
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
