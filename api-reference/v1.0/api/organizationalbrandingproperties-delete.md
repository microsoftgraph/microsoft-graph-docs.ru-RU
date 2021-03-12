---
title: Удаление organizationalBrandingProperties
description: Удаление организационных свойств.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4faef793d2ab02eb530ee839fdd683de04f4a179
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722658"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="27a2b-103">Удаление organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="27a2b-103">Delete organizationalBrandingProperties</span></span>

<span data-ttu-id="27a2b-104">Удаление [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="27a2b-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27a2b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27a2b-105">Permissions</span></span>

<span data-ttu-id="27a2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27a2b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27a2b-108">Permission type</span></span>                        | <span data-ttu-id="27a2b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a2b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27a2b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a2b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27a2b-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a2b-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="27a2b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a2b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a2b-113">Not supported.</span></span> |
| <span data-ttu-id="27a2b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27a2b-114">Application</span></span>                            | <span data-ttu-id="27a2b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a2b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27a2b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a2b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="27a2b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27a2b-117">Request headers</span></span>

| <span data-ttu-id="27a2b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="27a2b-118">Name</span></span>          | <span data-ttu-id="27a2b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="27a2b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27a2b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27a2b-120">Authorization</span></span> | <span data-ttu-id="27a2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27a2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27a2b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27a2b-123">Request body</span></span>

<span data-ttu-id="27a2b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27a2b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27a2b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a2b-125">Response</span></span>

<span data-ttu-id="27a2b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="27a2b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27a2b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="27a2b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27a2b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a2b-129">Request</span></span>

<span data-ttu-id="27a2b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27a2b-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

### <a name="response"></a><span data-ttu-id="27a2b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a2b-131">Response</span></span>

<span data-ttu-id="27a2b-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="27a2b-132">The following is an example of the response.</span></span>

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
