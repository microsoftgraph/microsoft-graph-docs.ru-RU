---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 761849207983157a770c6c9cd5bea90a6c1b14ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503063"
---
# <a name="remove-owner"></a><span data-ttu-id="e2ef6-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="e2ef6-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2ef6-104">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2ef6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ef6-105">Permissions</span></span>
<span data-ttu-id="e2ef6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2ef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2ef6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ef6-108">Permission type</span></span>      | <span data-ttu-id="e2ef6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2ef6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2ef6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2ef6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2ef6-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2ef6-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2ef6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2ef6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2ef6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-113">Not supported.</span></span>    |
|<span data-ttu-id="e2ef6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2ef6-114">Application</span></span> | <span data-ttu-id="e2ef6-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ef6-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2ef6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2ef6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e2ef6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2ef6-117">Request headers</span></span>
| <span data-ttu-id="e2ef6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e2ef6-118">Name</span></span>       | <span data-ttu-id="e2ef6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ef6-119">Type</span></span> | <span data-ttu-id="e2ef6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ef6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2ef6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2ef6-121">Authorization</span></span>  | <span data-ttu-id="e2ef6-122">string</span><span class="sxs-lookup"><span data-stu-id="e2ef6-122">string</span></span>  | <span data-ttu-id="e2ef6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2ef6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2ef6-125">Request body</span></span>
<span data-ttu-id="e2ef6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2ef6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ef6-127">Response</span></span>
<span data-ttu-id="e2ef6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2ef6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e2ef6-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e2ef6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2ef6-131">Request</span></span>
<span data-ttu-id="e2ef6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="e2ef6-133">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="e2ef6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ef6-134">Response</span></span>
<span data-ttu-id="e2ef6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-135">The following is an example of the response.</span></span>
><span data-ttu-id="e2ef6-136">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2ef6-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2ef6-137">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
