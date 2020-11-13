---
title: Удаление Организатионалбрандингпропертиес
description: Удаление Организатионалбрандингпропертиес.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c698becef5cb0ca7950ba9c210356aa76ee1814
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031997"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="82c92-103">Удаление Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="82c92-103">Delete organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82c92-104">Удаление объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="82c92-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82c92-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82c92-105">Permissions</span></span>

<span data-ttu-id="82c92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82c92-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82c92-108">Permission type</span></span>                        | <span data-ttu-id="82c92-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82c92-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82c92-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82c92-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82c92-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c92-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="82c92-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82c92-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82c92-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c92-113">Not supported.</span></span> |
| <span data-ttu-id="82c92-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82c92-114">Application</span></span>                            | <span data-ttu-id="82c92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c92-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82c92-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82c92-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="82c92-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82c92-117">Request headers</span></span>

| <span data-ttu-id="82c92-118">Имя</span><span class="sxs-lookup"><span data-stu-id="82c92-118">Name</span></span>          | <span data-ttu-id="82c92-119">Описание</span><span class="sxs-lookup"><span data-stu-id="82c92-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="82c92-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82c92-120">Authorization</span></span> | <span data-ttu-id="82c92-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82c92-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82c92-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82c92-123">Request body</span></span>

<span data-ttu-id="82c92-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82c92-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82c92-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c92-125">Response</span></span>

<span data-ttu-id="82c92-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="82c92-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82c92-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="82c92-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82c92-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="82c92-129">Request</span></span>

<span data-ttu-id="82c92-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82c92-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

### <a name="response"></a><span data-ttu-id="82c92-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c92-131">Response</span></span>

<span data-ttu-id="82c92-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="82c92-132">The following is an example of the response.</span></span>

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
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->