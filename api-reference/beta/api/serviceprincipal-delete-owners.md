---
title: Удаление владельца
description: Удаление владельца из СервицепринЦипалс.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bf9e90c8335ff73f5afe1a98f83ff6cb6502b720
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291331"
---
# <a name="remove-owner"></a><span data-ttu-id="af6c6-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="af6c6-103">Remove owner</span></span>

<span data-ttu-id="af6c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af6c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af6c6-105">Удаление владельца из объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="af6c6-105">Remove an owner from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af6c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af6c6-106">Permissions</span></span>
<span data-ttu-id="af6c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af6c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af6c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af6c6-109">Permission type</span></span>      | <span data-ttu-id="af6c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af6c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af6c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af6c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af6c6-112">Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="af6c6-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="af6c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af6c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af6c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af6c6-114">Not supported.</span></span>    |
|<span data-ttu-id="af6c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af6c6-115">Application</span></span> | <span data-ttu-id="af6c6-116">Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af6c6-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af6c6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af6c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /serviceprincipals/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="af6c6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af6c6-118">Request headers</span></span>
| <span data-ttu-id="af6c6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="af6c6-119">Name</span></span> | <span data-ttu-id="af6c6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="af6c6-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="af6c6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af6c6-121">Authorization</span></span> | <span data-ttu-id="af6c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af6c6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af6c6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af6c6-124">Request body</span></span>
<span data-ttu-id="af6c6-125">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="af6c6-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="af6c6-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="af6c6-126">Response</span></span>

<span data-ttu-id="af6c6-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af6c6-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="af6c6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="af6c6-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="af6c6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="af6c6-129">Request</span></span>

<span data-ttu-id="af6c6-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af6c6-130">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/serviceprincipals/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```

### <a name="response"></a><span data-ttu-id="af6c6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="af6c6-131">Response</span></span>

<span data-ttu-id="af6c6-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af6c6-132">The following is an example of the response.</span></span>

><span data-ttu-id="af6c6-133">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af6c6-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="af6c6-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af6c6-134">All the properties will be returned from an actual call.</span></span>

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
