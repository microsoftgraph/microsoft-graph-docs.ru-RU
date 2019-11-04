---
title: Удаление владельца
description: Удаление владельца из приложения.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 09db5c02123a788e9fee77753e60de961ea8fabf
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936568"
---
# <a name="remove-owner"></a><span data-ttu-id="2ff1a-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="2ff1a-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff1a-104">Удаление владельца из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="2ff1a-104">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ff1a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff1a-105">Permissions</span></span>
<span data-ttu-id="2ff1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ff1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ff1a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff1a-108">Permission type</span></span>      | <span data-ttu-id="2ff1a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ff1a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ff1a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ff1a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ff1a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ff1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ff1a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-113">Not supported.</span></span>    |
|<span data-ttu-id="2ff1a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ff1a-114">Application</span></span> | <span data-ttu-id="2ff1a-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ff1a-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ff1a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ff1a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="2ff1a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ff1a-117">Request headers</span></span>
| <span data-ttu-id="2ff1a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2ff1a-118">Name</span></span> | <span data-ttu-id="2ff1a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff1a-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="2ff1a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ff1a-120">Authorization</span></span> | <span data-ttu-id="2ff1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ff1a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ff1a-123">Request body</span></span>
<span data-ttu-id="2ff1a-124">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="2ff1a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ff1a-125">Response</span></span>

<span data-ttu-id="2ff1a-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ff1a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="2ff1a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ff1a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ff1a-128">Request</span></span>

<span data-ttu-id="2ff1a-129">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-129">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```

### <a name="response"></a><span data-ttu-id="2ff1a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ff1a-130">Response</span></span>

<span data-ttu-id="2ff1a-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-131">The following is an example of the response.</span></span>

><span data-ttu-id="2ff1a-132">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2ff1a-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ff1a-133">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
