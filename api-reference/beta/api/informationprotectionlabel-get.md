---
title: Получение Информатионпротектионлабел
description: Получение свойств и связей указанного объекта Информатионпротектионлабел.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bcd8c6e3d210615dec4d7bf4233256ab2cd5acb6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938536"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="c4ef3-103">Получение Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="c4ef3-103">Get informationProtectionLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4ef3-104">Получение свойств и связей объекта [информатионпротектионлабел](../resources/informationprotectionlabel.md) .</span><span class="sxs-lookup"><span data-stu-id="c4ef3-104">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4ef3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ef3-105">Permissions</span></span>

<span data-ttu-id="c4ef3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4ef3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ef3-108">Permission type</span></span>                        | <span data-ttu-id="c4ef3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4ef3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c4ef3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4ef3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4ef3-111">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="c4ef3-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="c4ef3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4ef3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ef3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-113">Not supported.</span></span>                              |
| <span data-ttu-id="c4ef3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4ef3-114">Application</span></span>                            | <span data-ttu-id="c4ef3-115">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c4ef3-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="c4ef3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4ef3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationprotection/policy/labels/{id}
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4ef3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4ef3-117">Optional query parameters</span></span>

<span data-ttu-id="c4ef3-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c4ef3-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c4ef3-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4ef3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4ef3-120">Request headers</span></span>

| <span data-ttu-id="c4ef3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c4ef3-121">Name</span></span>          | <span data-ttu-id="c4ef3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ef3-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="c4ef3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4ef3-123">Authorization</span></span> | <span data-ttu-id="c4ef3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="c4ef3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4ef3-126">Request body</span></span>

<span data-ttu-id="c4ef3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4ef3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4ef3-128">Response</span></span>

<span data-ttu-id="c4ef3-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [информатионпротектионлабел](../resources/informationprotectionlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-129">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4ef3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4ef3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4ef3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ef3-131">Request</span></span>

<span data-ttu-id="c4ef3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```http
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```

### <a name="response"></a><span data-ttu-id="c4ef3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ef3-133">Response</span></span>

<span data-ttu-id="c4ef3-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c4ef3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4ef3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels/$entity",
    "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
    "name": "LabelWithFooterAndHeaderActions_Tests",
    "description": "",
    "color": "",
    "sensitivity": 12,
    "tooltip": "LabelWithFooterAndHeaderActions_Tests",
    "isActive": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get informationProtectionLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
