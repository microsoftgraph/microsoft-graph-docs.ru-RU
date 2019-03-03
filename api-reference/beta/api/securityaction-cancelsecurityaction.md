---
title: 'securityAction: Канцелсекуритяктион'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1b37563ffde274944dc877482602c36d2bf3a4bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366954"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="616f0-103">securityAction: Канцелсекуритяктион</span><span class="sxs-lookup"><span data-stu-id="616f0-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="616f0-104">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="616f0-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="616f0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="616f0-105">Permissions</span></span>

<span data-ttu-id="616f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="616f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="616f0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="616f0-108">Permission type</span></span>                        | <span data-ttu-id="616f0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="616f0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="616f0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="616f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="616f0-111">Секуритяктионс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="616f0-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="616f0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="616f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="616f0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="616f0-113">Not supported.</span></span> |
| <span data-ttu-id="616f0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="616f0-114">Application</span></span>                            | <span data-ttu-id="616f0-115">Секуритяктионс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="616f0-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="616f0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="616f0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="616f0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="616f0-117">Request headers</span></span>

| <span data-ttu-id="616f0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="616f0-118">Name</span></span>          | <span data-ttu-id="616f0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="616f0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="616f0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="616f0-120">Authorization</span></span> | <span data-ttu-id="616f0-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="616f0-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="616f0-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="616f0-122">Request body</span></span>

<span data-ttu-id="616f0-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="616f0-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="616f0-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="616f0-124">Response</span></span>

<span data-ttu-id="616f0-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="616f0-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="616f0-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="616f0-127">Examples</span></span>

<span data-ttu-id="616f0-128">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="616f0-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="616f0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="616f0-129">Request</span></span>

<span data-ttu-id="616f0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="616f0-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="616f0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="616f0-131">Response</span></span>

<span data-ttu-id="616f0-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="616f0-132">The following is an example of the response.</span></span>
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
