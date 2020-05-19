---
title: 'servicePrincipal: Добавление владельца'
description: Добавьте владельца для субъекта службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 31851eb6e4e653d1c97ba56fda8c7a80e6e5803f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290014"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="9f6c5-103">servicePrincipal: Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="9f6c5-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="9f6c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f6c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f6c5-105">Добавьте владельца для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="9f6c5-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f6c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f6c5-106">Permissions</span></span>
<span data-ttu-id="9f6c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f6c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f6c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f6c5-109">Permission type</span></span>      | <span data-ttu-id="9f6c5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f6c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f6c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f6c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f6c5-112">Application. ReadWrite. ALL и Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9f6c5-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f6c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f6c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f6c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-114">Not supported.</span></span>    |
|<span data-ttu-id="9f6c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f6c5-115">Application</span></span> | <span data-ttu-id="9f6c5-116">Application. ReadWrite. Овнедби и Directory. Read. ALL, Application. ReadWrite. ALL и Directory. Read. ALL, Application. ReadWrite. Овнедби и Directory. ReadWrite. ALL, Application. ReadWrite. ALL и Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9f6c5-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9f6c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f6c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="9f6c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f6c5-118">Request headers</span></span>
| <span data-ttu-id="9f6c5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f6c5-119">Name</span></span>       | <span data-ttu-id="9f6c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f6c5-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="9f6c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f6c5-121">Authorization</span></span> | <span data-ttu-id="9f6c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f6c5-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f6c5-124">Request body</span></span>
<span data-ttu-id="9f6c5-125">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f6c5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f6c5-126">Response</span></span>

<span data-ttu-id="9f6c5-127">В случае успеха этот метод возвращает код отклика `204 No Content` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f6c5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f6c5-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="9f6c5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f6c5-129">Request</span></span>
<span data-ttu-id="9f6c5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-130">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

<span data-ttu-id="9f6c5-131">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-131">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="9f6c5-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f6c5-132">Response</span></span>
<span data-ttu-id="9f6c5-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9f6c5-133">The following is an example of the response.</span></span>

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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
