---
title: Удаление servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ff4806499b2c32b88ee87f6a1e33691e25f4f25a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291169"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="7304f-103">Удаление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="7304f-103">Delete servicePrincipal</span></span>

<span data-ttu-id="7304f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7304f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7304f-105">Удаление объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="7304f-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7304f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7304f-106">Permissions</span></span>
<span data-ttu-id="7304f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7304f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7304f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7304f-109">Permission type</span></span>      | <span data-ttu-id="7304f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7304f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7304f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7304f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7304f-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="7304f-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7304f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7304f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7304f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7304f-114">Not supported.</span></span>    |
|<span data-ttu-id="7304f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7304f-115">Application</span></span> | <span data-ttu-id="7304f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7304f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7304f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7304f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7304f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7304f-118">Request headers</span></span>
| <span data-ttu-id="7304f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7304f-119">Name</span></span>       | <span data-ttu-id="7304f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7304f-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7304f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7304f-121">Authorization</span></span> | <span data-ttu-id="7304f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7304f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7304f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7304f-124">Content-type</span></span> | <span data-ttu-id="7304f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7304f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7304f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7304f-127">Request body</span></span>
<span data-ttu-id="7304f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7304f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7304f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7304f-129">Response</span></span>

<span data-ttu-id="7304f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7304f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7304f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7304f-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="7304f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7304f-133">Request</span></span>
<span data-ttu-id="7304f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7304f-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
### <a name="response"></a><span data-ttu-id="7304f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7304f-135">Response</span></span>
<span data-ttu-id="7304f-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7304f-136">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
