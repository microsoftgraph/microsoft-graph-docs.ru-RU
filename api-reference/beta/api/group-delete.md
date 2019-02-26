---
title: Delete Group — API Microsoft Graph
description: Описывает метод Delete ресурса Group (Entity) API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 836f2c647fd9894a7d39bba80e5f15f3f11ef81f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255866"
---
# <a name="delete-group"></a><span data-ttu-id="0f500-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="0f500-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f500-104">Удаляет группу.</span><span class="sxs-lookup"><span data-stu-id="0f500-104">Deletes a group.</span></span>  

<span data-ttu-id="0f500-105">После удаления группы Office 365 перемещаются во временный контейнер и могут быть восстановлены в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="0f500-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="0f500-106">По исТечении этого времени они безвозвратно удаляются.</span><span class="sxs-lookup"><span data-stu-id="0f500-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="0f500-107">Дополнительные сведения см. в разделе [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="0f500-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="0f500-108">Это применимо только к группам Office 365.</span><span class="sxs-lookup"><span data-stu-id="0f500-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f500-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f500-109">Permissions</span></span>

<span data-ttu-id="0f500-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f500-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f500-112">Permission type</span></span>      | <span data-ttu-id="0f500-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f500-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f500-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f500-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0f500-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f500-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f500-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f500-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f500-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f500-117">Not supported.</span></span>    |
|<span data-ttu-id="0f500-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f500-118">Application</span></span> | <span data-ttu-id="0f500-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f500-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f500-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f500-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f500-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f500-121">Request headers</span></span>

| <span data-ttu-id="0f500-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0f500-122">Name</span></span>       | <span data-ttu-id="0f500-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0f500-123">Type</span></span> | <span data-ttu-id="0f500-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0f500-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f500-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f500-125">Authorization</span></span>  | <span data-ttu-id="0f500-126">строка</span><span class="sxs-lookup"><span data-stu-id="0f500-126">string</span></span>  | <span data-ttu-id="0f500-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f500-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f500-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f500-129">Request body</span></span>

<span data-ttu-id="0f500-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f500-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f500-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f500-131">Response</span></span>

<span data-ttu-id="0f500-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0f500-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f500-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0f500-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f500-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f500-135">Request</span></span>

<span data-ttu-id="0f500-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f500-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="0f500-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f500-137">Response</span></span>

<span data-ttu-id="0f500-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0f500-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
