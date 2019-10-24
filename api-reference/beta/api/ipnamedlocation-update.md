---
title: Обновление ипнамедлокатион
description: Обновление свойств объекта Ипнамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e9b1dfbe84124c6f6049260732bf254e98682870
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653722"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="84214-103">Обновление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="84214-103">Update ipNamedlocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84214-104">Обновление свойств объекта [ипнамедлокатион](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="84214-104">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84214-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84214-105">Permissions</span></span>

<span data-ttu-id="84214-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84214-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84214-108">Permission type</span></span>                        | <span data-ttu-id="84214-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84214-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84214-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84214-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="84214-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="84214-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="84214-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84214-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84214-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84214-113">Not supported.</span></span> |
| <span data-ttu-id="84214-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84214-114">Application</span></span>                            | <span data-ttu-id="84214-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84214-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="84214-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="84214-116">This API requires multiple permissions.</span></span> <span data-ttu-id="84214-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="84214-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="84214-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84214-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84214-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84214-119">Request headers</span></span>

| <span data-ttu-id="84214-120">Имя</span><span class="sxs-lookup"><span data-stu-id="84214-120">Name</span></span>       | <span data-ttu-id="84214-121">Описание</span><span class="sxs-lookup"><span data-stu-id="84214-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="84214-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84214-122">Authorization</span></span> | <span data-ttu-id="84214-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84214-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84214-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84214-125">Content-type</span></span> | <span data-ttu-id="84214-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84214-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84214-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84214-128">Request body</span></span>

<span data-ttu-id="84214-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="84214-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="84214-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="84214-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="84214-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="84214-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="84214-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="84214-132">Property</span></span>     | <span data-ttu-id="84214-133">Тип</span><span class="sxs-lookup"><span data-stu-id="84214-133">Type</span></span>        | <span data-ttu-id="84214-134">Описание</span><span class="sxs-lookup"><span data-stu-id="84214-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84214-135">displayName</span><span class="sxs-lookup"><span data-stu-id="84214-135">displayName</span></span>|<span data-ttu-id="84214-136">String</span><span class="sxs-lookup"><span data-stu-id="84214-136">String</span></span>|<span data-ttu-id="84214-137">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="84214-137">Human-readable name of the location.</span></span>|
|<span data-ttu-id="84214-138">ипранжес</span><span class="sxs-lookup"><span data-stu-id="84214-138">ipRanges</span></span>|<span data-ttu-id="84214-139">Коллекция объектов [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="84214-139">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="84214-140">Список диапазонов IP-адресов в формате IPv4 CIDR (1.2.3.4/32) или любом допустимом формате IPv6 из IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="84214-140">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="84214-141">Доверять</span><span class="sxs-lookup"><span data-stu-id="84214-141">isTrusted</span></span>|<span data-ttu-id="84214-142">Логический</span><span class="sxs-lookup"><span data-stu-id="84214-142">Boolean</span></span>|<span data-ttu-id="84214-143">Значение, `true` если это расположение явно доверенное.</span><span class="sxs-lookup"><span data-stu-id="84214-143">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="84214-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="84214-144">Response</span></span>

<span data-ttu-id="84214-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="84214-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84214-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="84214-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84214-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="84214-148">Request</span></span>

<span data-ttu-id="84214-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84214-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84214-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="84214-150">Response</span></span>

<span data-ttu-id="84214-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84214-151">The following is an example of the response.</span></span>

> <span data-ttu-id="84214-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84214-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
