---
title: Удаление объекта inferenceClassificationOverride
description: Удаление переопределения по идентификатору.
localization_priority: Normal
ms.openlocfilehash: 303593fd666d24e2d3a1b095898c9756afd850bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832894"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="13f55-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="13f55-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="13f55-104">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="13f55-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="13f55-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13f55-105">Permissions</span></span>
<span data-ttu-id="13f55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13f55-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13f55-108">Permission type</span></span>      | <span data-ttu-id="13f55-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13f55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13f55-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13f55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13f55-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13f55-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13f55-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13f55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13f55-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13f55-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="13f55-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13f55-114">Application</span></span> | <span data-ttu-id="13f55-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13f55-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13f55-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13f55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="13f55-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13f55-117">Request headers</span></span>
| <span data-ttu-id="13f55-118">Имя</span><span class="sxs-lookup"><span data-stu-id="13f55-118">Name</span></span>       | <span data-ttu-id="13f55-119">Тип</span><span class="sxs-lookup"><span data-stu-id="13f55-119">Type</span></span> | <span data-ttu-id="13f55-120">Описание</span><span class="sxs-lookup"><span data-stu-id="13f55-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13f55-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="13f55-121">Authorization</span></span>  | <span data-ttu-id="13f55-122">string</span><span class="sxs-lookup"><span data-stu-id="13f55-122">string</span></span>  | <span data-ttu-id="13f55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13f55-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13f55-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13f55-125">Request body</span></span>
<span data-ttu-id="13f55-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13f55-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13f55-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="13f55-127">Response</span></span>

<span data-ttu-id="13f55-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="13f55-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13f55-130">Пример</span><span class="sxs-lookup"><span data-stu-id="13f55-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13f55-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="13f55-131">Request</span></span>
<span data-ttu-id="13f55-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13f55-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="13f55-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="13f55-133">Response</span></span>
<span data-ttu-id="13f55-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="13f55-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
