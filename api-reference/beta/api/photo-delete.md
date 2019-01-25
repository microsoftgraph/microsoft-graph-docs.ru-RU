---
title: Удаление фотографии
description: Удаление фотографии.
localization_priority: Normal
ms.openlocfilehash: 8f29f272aeaebd8aed7de14b817d3e4c7719f511
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526930"
---
# <a name="delete-photo"></a><span data-ttu-id="e8d9f-103">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="e8d9f-103">Delete photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8d9f-104">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8d9f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8d9f-105">Permissions</span></span>
<span data-ttu-id="e8d9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d9f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8d9f-108">Permission type</span></span>      | <span data-ttu-id="e8d9f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8d9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d9f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8d9f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8d9f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8d9f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8d9f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8d9f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d9f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8d9f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8d9f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8d9f-114">Application</span></span> | <span data-ttu-id="e8d9f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8d9f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8d9f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="e8d9f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8d9f-117">Request headers</span></span>
| <span data-ttu-id="e8d9f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e8d9f-118">Name</span></span>       | <span data-ttu-id="e8d9f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e8d9f-119">Type</span></span> | <span data-ttu-id="e8d9f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8d9f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8d9f-121">if-match</span><span class="sxs-lookup"><span data-stu-id="e8d9f-121">if-match</span></span>  | <span data-ttu-id="e8d9f-122">string</span><span class="sxs-lookup"><span data-stu-id="e8d9f-122">string</span></span>  | <span data-ttu-id="e8d9f-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="e8d9f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8d9f-124">Authorization</span></span>  | <span data-ttu-id="e8d9f-125">string</span><span class="sxs-lookup"><span data-stu-id="e8d9f-125">string</span></span>  | <span data-ttu-id="e8d9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8d9f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8d9f-128">Request body</span></span>
<span data-ttu-id="e8d9f-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8d9f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8d9f-130">Response</span></span>

<span data-ttu-id="e8d9f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8d9f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e8d9f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8d9f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8d9f-134">Request</span></span>
<span data-ttu-id="e8d9f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="e8d9f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8d9f-136">Response</span></span>
<span data-ttu-id="e8d9f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8d9f-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/photo-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
