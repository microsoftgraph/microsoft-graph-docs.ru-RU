---
title: 'securityAction: Канцелсекуритяктион'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: be737b6c1f6a8421cc87a7dd8efc222b48d7c078
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545717"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="307fb-103">securityAction: Канцелсекуритяктион</span><span class="sxs-lookup"><span data-stu-id="307fb-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="307fb-104">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="307fb-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="307fb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="307fb-105">Permissions</span></span>

<span data-ttu-id="307fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="307fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="307fb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="307fb-108">Permission type</span></span>                        | <span data-ttu-id="307fb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="307fb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="307fb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="307fb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="307fb-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="307fb-111">Not supported.</span></span> |
| <span data-ttu-id="307fb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="307fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="307fb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="307fb-113">Not supported.</span></span> |
| <span data-ttu-id="307fb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="307fb-114">Application</span></span>                            | <span data-ttu-id="307fb-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="307fb-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="307fb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="307fb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="307fb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="307fb-117">Request headers</span></span>

| <span data-ttu-id="307fb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="307fb-118">Name</span></span>          | <span data-ttu-id="307fb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="307fb-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="307fb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="307fb-120">Authorization</span></span> | <span data-ttu-id="307fb-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="307fb-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="307fb-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="307fb-122">Request body</span></span>

<span data-ttu-id="307fb-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="307fb-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="307fb-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="307fb-124">Response</span></span>

<span data-ttu-id="307fb-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="307fb-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="307fb-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="307fb-127">Examples</span></span>

<span data-ttu-id="307fb-128">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="307fb-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="307fb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="307fb-129">Request</span></span>

<span data-ttu-id="307fb-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="307fb-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="307fb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="307fb-131">Response</span></span>

<span data-ttu-id="307fb-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="307fb-132">The following is an example of the response.</span></span>
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
