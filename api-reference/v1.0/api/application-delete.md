---
title: Удаление приложения
description: Удаление объекта Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ecaafbaaa8558d8e9d86d45a75f824272fb6a14
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939735"
---
# <a name="delete-application"></a><span data-ttu-id="10f99-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="10f99-103">Delete application</span></span>

<span data-ttu-id="10f99-104">Удаление объекта [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="10f99-104">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10f99-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10f99-105">Permissions</span></span>
<span data-ttu-id="10f99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f99-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10f99-108">Permission type</span></span>      | <span data-ttu-id="10f99-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10f99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10f99-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10f99-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10f99-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10f99-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10f99-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10f99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10f99-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10f99-113">Not supported.</span></span>    |
|<span data-ttu-id="10f99-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10f99-114">Application</span></span> | <span data-ttu-id="10f99-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f99-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10f99-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10f99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="10f99-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10f99-117">Request headers</span></span>
| <span data-ttu-id="10f99-118">Имя</span><span class="sxs-lookup"><span data-stu-id="10f99-118">Name</span></span>       | <span data-ttu-id="10f99-119">Тип</span><span class="sxs-lookup"><span data-stu-id="10f99-119">Type</span></span> | <span data-ttu-id="10f99-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10f99-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10f99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10f99-121">Authorization</span></span>  | <span data-ttu-id="10f99-122">string</span><span class="sxs-lookup"><span data-stu-id="10f99-122">string</span></span>  | <span data-ttu-id="10f99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10f99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10f99-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10f99-125">Request body</span></span>
<span data-ttu-id="10f99-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10f99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10f99-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="10f99-127">Response</span></span>

<span data-ttu-id="10f99-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10f99-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f99-130">Пример</span><span class="sxs-lookup"><span data-stu-id="10f99-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10f99-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="10f99-131">Request</span></span>
<span data-ttu-id="10f99-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10f99-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```

##### <a name="response"></a><span data-ttu-id="10f99-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="10f99-133">Response</span></span>
<span data-ttu-id="10f99-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10f99-134">Here is an example of the response.</span></span> 
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
  ]
}
-->
