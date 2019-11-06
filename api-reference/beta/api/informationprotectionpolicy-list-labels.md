---
title: 'Информатионпротектионлабел: Листлабелс'
description: Получение списка меток защиты информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ceadfa6a1db960e7ca9f394df51233f792ec98f9
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994396"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="459b1-103">Информатионпротектионлабел: Листлабелс</span><span class="sxs-lookup"><span data-stu-id="459b1-103">informationProtectionLabel: listLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="459b1-104">Получение набора [меток защиты информации](../resources/informationprotectionlabel.md) , доступных пользователю или организации.</span><span class="sxs-lookup"><span data-stu-id="459b1-104">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="459b1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="459b1-105">Permissions</span></span>

<span data-ttu-id="459b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="459b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="459b1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="459b1-108">Permission type</span></span>                        | <span data-ttu-id="459b1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="459b1-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="459b1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="459b1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="459b1-111">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="459b1-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="459b1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="459b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="459b1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="459b1-113">Not supported.</span></span>                              |
| <span data-ttu-id="459b1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="459b1-114">Application</span></span>                            | <span data-ttu-id="459b1-115">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="459b1-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="459b1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="459b1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/informationprotection/policy/labels
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="459b1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="459b1-117">Optional query parameters</span></span>

<span data-ttu-id="459b1-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="459b1-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="459b1-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="459b1-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="459b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="459b1-120">Request headers</span></span>

| <span data-ttu-id="459b1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="459b1-121">Name</span></span>          | <span data-ttu-id="459b1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="459b1-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="459b1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="459b1-123">Authorization</span></span> | <span data-ttu-id="459b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="459b1-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="459b1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="459b1-126">Request body</span></span>

<span data-ttu-id="459b1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="459b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="459b1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="459b1-128">Response</span></span>

<span data-ttu-id="459b1-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [информатионпротектионлабел](../resources/informationprotectionlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="459b1-129">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="459b1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="459b1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="459b1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="459b1-131">Request</span></span>

<span data-ttu-id="459b1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="459b1-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="459b1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="459b1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="459b1-134">C#</span><span class="sxs-lookup"><span data-stu-id="459b1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="459b1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="459b1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="459b1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="459b1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="459b1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="459b1-137">Response</span></span>

<span data-ttu-id="459b1-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="459b1-138">The following is an example of the response.</span></span>

> <span data-ttu-id="459b1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="459b1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels",
  "value": [
      {
          "id": "3a80e051-487c-40d4-b491-73ad25d997e6",
          "name": "General",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 1,
          "tooltip": "Data classified as Contoso General.",
          "isActive": true
      },
      {
          "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
          "name": "Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 2,
          "tooltip": "Data classificed as Contoso Confidential.",
          "isActive": true
      },
      {
          "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
          "name": "Highly Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 3,
          "tooltip": "Data classified as Contoso Highly Confidential.",
          "isActive": true
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List labels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
