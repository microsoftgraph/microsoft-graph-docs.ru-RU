---
title: Удаление индикатора службы угроз
description: Удаление объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: eac07b5d3e81e3e3098fb63bbf0be838c7d51b2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537050"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="7dcc1-103">Удаление индикатора службы угроз</span><span class="sxs-lookup"><span data-stu-id="7dcc1-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dcc1-104">Удаление объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="7dcc1-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dcc1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dcc1-105">Permissions</span></span>

<span data-ttu-id="7dcc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dcc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dcc1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dcc1-108">Permission type</span></span>                        | <span data-ttu-id="7dcc1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dcc1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7dcc1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dcc1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dcc1-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7dcc1-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="7dcc1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dcc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dcc1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dcc1-113">Not supported.</span></span> |
| <span data-ttu-id="7dcc1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dcc1-114">Application</span></span>                            | <span data-ttu-id="7dcc1-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7dcc1-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dcc1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dcc1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7dcc1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dcc1-117">Request headers</span></span>

| <span data-ttu-id="7dcc1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7dcc1-118">Name</span></span>          | <span data-ttu-id="7dcc1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7dcc1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7dcc1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7dcc1-120">Authorization</span></span> | <span data-ttu-id="7dcc1-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7dcc1-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dcc1-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7dcc1-122">Request body</span></span>

<span data-ttu-id="7dcc1-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7dcc1-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dcc1-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dcc1-124">Response</span></span>

<span data-ttu-id="7dcc1-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7dcc1-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7dcc1-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="7dcc1-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7dcc1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dcc1-128">Request</span></span>

<span data-ttu-id="7dcc1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dcc1-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="7dcc1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dcc1-130">Response</span></span>

<span data-ttu-id="7dcc1-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7dcc1-131">The following is an example of the response.</span></span>

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
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
