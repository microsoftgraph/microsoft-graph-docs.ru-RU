---
title: Удаление локализованных организационных свойствBrandingProperties
description: Удаление организационных свойств для определенной локализации.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d15d5e5ef20cc7d18fbd26097fcdc19f7802ca0f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722640"
---
# <a name="delete-localized-organizationalbrandingproperties"></a><span data-ttu-id="2a5b2-103">Удаление локализованных организационных свойствBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="2a5b2-103">Delete Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="2a5b2-104">Удаление [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="2a5b2-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a5b2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a5b2-105">Permissions</span></span>

<span data-ttu-id="2a5b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a5b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a5b2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a5b2-108">Permission type</span></span>                        | <span data-ttu-id="2a5b2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a5b2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a5b2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a5b2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a5b2-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a5b2-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="2a5b2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a5b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a5b2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-113">Not supported.</span></span> |
| <span data-ttu-id="2a5b2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a5b2-114">Application</span></span>                            | <span data-ttu-id="2a5b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a5b2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a5b2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="2a5b2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a5b2-117">Request headers</span></span>

| <span data-ttu-id="2a5b2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2a5b2-118">Name</span></span>          | <span data-ttu-id="2a5b2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2a5b2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a5b2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a5b2-120">Authorization</span></span> | <span data-ttu-id="2a5b2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a5b2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a5b2-123">Request body</span></span>

<span data-ttu-id="2a5b2-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a5b2-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a5b2-125">Response</span></span>

<span data-ttu-id="2a5b2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a5b2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a5b2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a5b2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a5b2-129">Request</span></span>

<span data-ttu-id="2a5b2-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

### <a name="response"></a><span data-ttu-id="2a5b2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a5b2-131">Response</span></span>

<span data-ttu-id="2a5b2-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a5b2-132">The following is an example of the response.</span></span>

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
