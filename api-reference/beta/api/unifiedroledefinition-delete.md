---
title: Удаление Унифиедроледефинитион
description: Удаление объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e0d097732c58285c50004c4416e602960106acb
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437848"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="f9503-103">Удаление Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="f9503-103">Delete unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9503-104">Удаление объекта [унифиедроледефинитион](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f9503-104">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9503-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9503-105">Permissions</span></span>

<span data-ttu-id="f9503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9503-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9503-108">Permission type</span></span>                        | <span data-ttu-id="f9503-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9503-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9503-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9503-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9503-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="f9503-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="f9503-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9503-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9503-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9503-113">Not supported.</span></span> |
| <span data-ttu-id="f9503-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9503-114">Application</span></span>                            | <span data-ttu-id="f9503-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="f9503-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9503-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9503-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="f9503-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9503-117">Request headers</span></span>

| <span data-ttu-id="f9503-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f9503-118">Name</span></span>          | <span data-ttu-id="f9503-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f9503-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f9503-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9503-120">Authorization</span></span> | <span data-ttu-id="f9503-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f9503-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9503-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9503-122">Request body</span></span>

<span data-ttu-id="f9503-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9503-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9503-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9503-124">Response</span></span>

<span data-ttu-id="f9503-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f9503-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9503-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f9503-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9503-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9503-128">Request</span></span>

<span data-ttu-id="f9503-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9503-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```

### <a name="response"></a><span data-ttu-id="f9503-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9503-130">Response</span></span>

<span data-ttu-id="f9503-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f9503-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->