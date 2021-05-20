---
title: Обновление проверки подлинностиContextClassReference
description: Обновление свойств объекта authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dcc0a20ac8b10fc1b7fad3fa3472832036f70024
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547434"
---
# <a name="update-authenticationcontextclassreference"></a><span data-ttu-id="919c1-103">Обновление проверки подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="919c1-103">Update authenticationContextClassReference</span></span>

<span data-ttu-id="919c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="919c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="919c1-105">Обновление свойств объекта [authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="919c1-105">Update the properties of an [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="919c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="919c1-106">Permissions</span></span>

<span data-ttu-id="919c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="919c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="919c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="919c1-109">Permission type</span></span>                        | <span data-ttu-id="919c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="919c1-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="919c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="919c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="919c1-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="919c1-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="919c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="919c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="919c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="919c1-114">Not supported.</span></span> |
|<span data-ttu-id="919c1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="919c1-115">Application</span></span>                            | <span data-ttu-id="919c1-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="919c1-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="919c1-117">Этот API имеет [известные проблемы, связанные](/graph/known-issues#permissions) с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="919c1-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="919c1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="919c1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/authenticationContextClassReferences/{id}
```

## <a name="request-headers"></a><span data-ttu-id="919c1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="919c1-119">Request headers</span></span>

| <span data-ttu-id="919c1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="919c1-120">Name</span></span>          | <span data-ttu-id="919c1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="919c1-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="919c1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="919c1-122">Authorization</span></span> | <span data-ttu-id="919c1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="919c1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="919c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="919c1-125">Content-Type</span></span>  | <span data-ttu-id="919c1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="919c1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="919c1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="919c1-128">Request body</span></span>

<span data-ttu-id="919c1-129">В теле запроса укажи значения для соответствующих свойств, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="919c1-129">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="919c1-130">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="919c1-130">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="919c1-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="919c1-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="919c1-132">Список свойств см. в списке [authenticationContextClassReference.](../resources/authenticationContextClassReference.md)</span><span class="sxs-lookup"><span data-stu-id="919c1-132">For the list of properties, see [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="response"></a><span data-ttu-id="919c1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="919c1-133">Response</span></span>

<span data-ttu-id="919c1-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="919c1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="919c1-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="919c1-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="919c1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="919c1-137">Request</span></span>

<span data-ttu-id="919c1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="919c1-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authenticationcontextclassreference"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
Content-type: application/json

{
   "value": 
    [
      {
         "displayName": "Contoso trusted locations",
        "description": "Access is only allowed from trusted locations",
        "isAvailable": true
      }
    ]
}
```



### <a name="response"></a><span data-ttu-id="919c1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="919c1-139">Response</span></span>

<span data-ttu-id="919c1-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="919c1-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
