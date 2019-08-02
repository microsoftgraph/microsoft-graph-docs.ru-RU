---
title: Удаление appliesTo
description: Удаление directoryObject из развертывания компонента.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1247cc352103bce040dc994feccd23ab9ba5a1bc
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062167"
---
# <a name="remove-appliesto"></a><span data-ttu-id="ffd25-103">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="ffd25-103">Remove appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffd25-104">Удалите элемент appliesTo в объекте [феатурероллаутполици](../resources/featurerolloutpolicy.md) , чтобы удалить [directoryObject](../resources/directoryobject.md) из развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="ffd25-104">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffd25-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd25-105">Permissions</span></span>

<span data-ttu-id="ffd25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ffd25-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd25-108">Permission type</span></span>                        | <span data-ttu-id="ffd25-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffd25-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ffd25-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffd25-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffd25-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="ffd25-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="ffd25-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffd25-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffd25-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd25-113">Not supported.</span></span> |
| <span data-ttu-id="ffd25-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffd25-114">Application</span></span>                            | <span data-ttu-id="ffd25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd25-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffd25-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffd25-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}/appliesTo/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ffd25-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffd25-117">Request headers</span></span>

| <span data-ttu-id="ffd25-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ffd25-118">Name</span></span>          | <span data-ttu-id="ffd25-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ffd25-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ffd25-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffd25-120">Authorization</span></span> | <span data-ttu-id="ffd25-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ffd25-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffd25-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffd25-122">Request body</span></span>

<span data-ttu-id="ffd25-123">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffd25-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ffd25-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd25-124">Response</span></span>

<span data-ttu-id="ffd25-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ffd25-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffd25-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="ffd25-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ffd25-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffd25-128">Request</span></span>

<span data-ttu-id="ffd25-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffd25-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```

### <a name="response"></a><span data-ttu-id="ffd25-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd25-130">Response</span></span>

<span data-ttu-id="ffd25-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd25-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->