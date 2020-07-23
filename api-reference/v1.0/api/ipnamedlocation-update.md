---
title: Обновление ипнамедлокатион
description: Обновление свойств объекта Ипнамедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b385c8ce1c86a6dee3116afd68681470097bbc48
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384819"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="3845c-103">Обновление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3845c-103">Update ipNamedlocation</span></span>

<span data-ttu-id="3845c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3845c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3845c-105">Обновление свойств объекта [ипнамедлокатион](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="3845c-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3845c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3845c-106">Permissions</span></span>

<span data-ttu-id="3845c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3845c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3845c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3845c-109">Permission type</span></span>                        | <span data-ttu-id="3845c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3845c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3845c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3845c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3845c-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="3845c-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="3845c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3845c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3845c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3845c-114">Not supported.</span></span> |
| <span data-ttu-id="3845c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3845c-115">Application</span></span>                            | <span data-ttu-id="3845c-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="3845c-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="3845c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3845c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3845c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3845c-118">Request headers</span></span>

| <span data-ttu-id="3845c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3845c-119">Name</span></span>       | <span data-ttu-id="3845c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3845c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3845c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3845c-121">Authorization</span></span> | <span data-ttu-id="3845c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3845c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3845c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3845c-124">Content-type</span></span> | <span data-ttu-id="3845c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3845c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3845c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3845c-127">Request body</span></span>

<span data-ttu-id="3845c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3845c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3845c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3845c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3845c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3845c-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3845c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="3845c-131">Property</span></span>     | <span data-ttu-id="3845c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3845c-132">Type</span></span>        | <span data-ttu-id="3845c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3845c-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3845c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3845c-134">displayName</span></span>|<span data-ttu-id="3845c-135">String</span><span class="sxs-lookup"><span data-stu-id="3845c-135">String</span></span>|<span data-ttu-id="3845c-136">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="3845c-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="3845c-137">ипранжес</span><span class="sxs-lookup"><span data-stu-id="3845c-137">ipRanges</span></span>|<span data-ttu-id="3845c-138">Коллекция объектов [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3845c-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="3845c-139">Список диапазонов IP-адресов в формате IPv4 CIDR (1.2.3.4/32) или любом допустимом формате IPv6 из IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="3845c-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="3845c-140">Доверять</span><span class="sxs-lookup"><span data-stu-id="3845c-140">isTrusted</span></span>|<span data-ttu-id="3845c-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="3845c-141">Boolean</span></span>|<span data-ttu-id="3845c-142">Значение, `true` если это расположение явно доверенное.</span><span class="sxs-lookup"><span data-stu-id="3845c-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="3845c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3845c-143">Response</span></span>

<span data-ttu-id="3845c-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3845c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3845c-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="3845c-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3845c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="3845c-147">Request</span></span>

<span data-ttu-id="3845c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3845c-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
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

### <a name="response"></a><span data-ttu-id="3845c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3845c-149">Response</span></span>

<span data-ttu-id="3845c-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3845c-150">The following is an example of the response.</span></span>

> <span data-ttu-id="3845c-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3845c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
