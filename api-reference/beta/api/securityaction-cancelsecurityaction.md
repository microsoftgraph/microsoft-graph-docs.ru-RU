---
title: 'securityAction: Канцелсекуритяктион'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: be737b6c1f6a8421cc87a7dd8efc222b48d7c078
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331455"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="7e51b-103">securityAction: Канцелсекуритяктион</span><span class="sxs-lookup"><span data-stu-id="7e51b-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e51b-104">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="7e51b-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e51b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e51b-105">Permissions</span></span>

<span data-ttu-id="7e51b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e51b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e51b-108">Permission type</span></span>                        | <span data-ttu-id="7e51b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e51b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e51b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e51b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e51b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e51b-111">Not supported.</span></span> |
| <span data-ttu-id="7e51b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e51b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e51b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e51b-113">Not supported.</span></span> |
| <span data-ttu-id="7e51b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e51b-114">Application</span></span>                            | <span data-ttu-id="7e51b-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e51b-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e51b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e51b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="7e51b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e51b-117">Request headers</span></span>

| <span data-ttu-id="7e51b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e51b-118">Name</span></span>          | <span data-ttu-id="7e51b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e51b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7e51b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e51b-120">Authorization</span></span> | <span data-ttu-id="7e51b-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7e51b-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e51b-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e51b-122">Request body</span></span>

<span data-ttu-id="7e51b-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e51b-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e51b-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e51b-124">Response</span></span>

<span data-ttu-id="7e51b-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7e51b-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e51b-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e51b-127">Examples</span></span>

<span data-ttu-id="7e51b-128">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="7e51b-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7e51b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e51b-129">Request</span></span>

<span data-ttu-id="7e51b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e51b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="7e51b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e51b-131">Response</span></span>

<span data-ttu-id="7e51b-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e51b-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
