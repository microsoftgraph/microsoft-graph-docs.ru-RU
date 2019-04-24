---
title: Удаление приложения
description: Удаляет приложение.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7db745e77125049a8a2e2c225c35c888e594451a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459246"
---
# <a name="delete-application"></a><span data-ttu-id="51579-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="51579-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51579-104">Удаляет приложение.</span><span class="sxs-lookup"><span data-stu-id="51579-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="51579-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51579-105">Permissions</span></span>
<span data-ttu-id="51579-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51579-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51579-108">Permission type</span></span>      | <span data-ttu-id="51579-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51579-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51579-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51579-110">Delegated (work or school account)</span></span> | <span data-ttu-id="51579-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51579-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51579-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51579-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51579-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51579-113">Not supported.</span></span>    |
|<span data-ttu-id="51579-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51579-114">Application</span></span> | <span data-ttu-id="51579-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51579-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51579-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51579-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="51579-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51579-117">Request headers</span></span>
| <span data-ttu-id="51579-118">Имя</span><span class="sxs-lookup"><span data-stu-id="51579-118">Name</span></span>       | <span data-ttu-id="51579-119">Тип</span><span class="sxs-lookup"><span data-stu-id="51579-119">Type</span></span> | <span data-ttu-id="51579-120">Описание</span><span class="sxs-lookup"><span data-stu-id="51579-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51579-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51579-121">Authorization</span></span>  | <span data-ttu-id="51579-122">string</span><span class="sxs-lookup"><span data-stu-id="51579-122">string</span></span>  | <span data-ttu-id="51579-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51579-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51579-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51579-125">Request body</span></span>
<span data-ttu-id="51579-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51579-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51579-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="51579-127">Response</span></span>

<span data-ttu-id="51579-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="51579-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51579-130">Пример</span><span class="sxs-lookup"><span data-stu-id="51579-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51579-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="51579-131">Request</span></span>
<span data-ttu-id="51579-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51579-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="51579-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="51579-133">Response</span></span>
<span data-ttu-id="51579-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51579-134">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
