---
title: Обновление ипнамедлокатион
description: Обновление свойств объекта Ипнамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de1811094d6be3148610078d25e0afafecc3fb04
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636850"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="e0aae-103">Обновление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="e0aae-103">Update ipNamedlocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0aae-104">Обновление свойств объекта [ипнамедлокатион](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="e0aae-104">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0aae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0aae-105">Permissions</span></span>

<span data-ttu-id="e0aae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0aae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0aae-108">Permission type</span></span>                        | <span data-ttu-id="e0aae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0aae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0aae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0aae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0aae-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="e0aae-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="e0aae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0aae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0aae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0aae-113">Not supported.</span></span> |
| <span data-ttu-id="e0aae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0aae-114">Application</span></span>                            | <span data-ttu-id="e0aae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0aae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0aae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0aae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0aae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0aae-117">Request headers</span></span>

| <span data-ttu-id="e0aae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e0aae-118">Name</span></span>       | <span data-ttu-id="e0aae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e0aae-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e0aae-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0aae-120">Authorization</span></span> | <span data-ttu-id="e0aae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0aae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0aae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0aae-123">Content-type</span></span> | <span data-ttu-id="e0aae-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0aae-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0aae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0aae-126">Request body</span></span>

<span data-ttu-id="e0aae-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e0aae-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e0aae-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e0aae-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e0aae-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e0aae-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0aae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0aae-130">Property</span></span>     | <span data-ttu-id="e0aae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e0aae-131">Type</span></span>        | <span data-ttu-id="e0aae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e0aae-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0aae-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e0aae-133">displayName</span></span>|<span data-ttu-id="e0aae-134">String</span><span class="sxs-lookup"><span data-stu-id="e0aae-134">String</span></span>|<span data-ttu-id="e0aae-135">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="e0aae-135">Human-readable name of the location.</span></span>|
|<span data-ttu-id="e0aae-136">ипранжес</span><span class="sxs-lookup"><span data-stu-id="e0aae-136">ipRanges</span></span>|<span data-ttu-id="e0aae-137">Коллекция объектов [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e0aae-137">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="e0aae-138">Список диапазонов IP-адресов в формате IPv4 CIDR (1.2.3.4/32) или любом допустимом формате IPv6 из IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="e0aae-138">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="e0aae-139">Доверять</span><span class="sxs-lookup"><span data-stu-id="e0aae-139">isTrusted</span></span>|<span data-ttu-id="e0aae-140">Логический</span><span class="sxs-lookup"><span data-stu-id="e0aae-140">Boolean</span></span>|<span data-ttu-id="e0aae-141">Значение, `true` если это расположение явно доверенное.</span><span class="sxs-lookup"><span data-stu-id="e0aae-141">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="e0aae-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0aae-142">Response</span></span>

<span data-ttu-id="e0aae-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0aae-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0aae-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0aae-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0aae-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0aae-146">Request</span></span>

<span data-ttu-id="e0aae-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0aae-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e0aae-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0aae-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted named location with only IPv4 address",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "6.5.4.3/18"
        }

    ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0aae-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0aae-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0aae-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0aae-150">Response</span></span>

<span data-ttu-id="e0aae-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0aae-151">The following is an example of the response.</span></span>

> <span data-ttu-id="e0aae-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0aae-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ipnamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
