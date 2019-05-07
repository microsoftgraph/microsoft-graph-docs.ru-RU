---
title: Удаление соглашения
description: Удаление объекта соглашения.
localization_priority: Normal
ms.openlocfilehash: ae2326f3ff2d1b13c4b4401a07b116db2e47876e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636599"
---
# <a name="delete-agreement"></a><span data-ttu-id="7ee95-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="7ee95-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ee95-104">Удаление объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="7ee95-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ee95-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ee95-105">Permissions</span></span>
<span data-ttu-id="7ee95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ee95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ee95-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ee95-108">Permission type</span></span>                        | <span data-ttu-id="7ee95-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ee95-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ee95-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ee95-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ee95-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ee95-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="7ee95-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ee95-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ee95-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ee95-113">Not supported.</span></span> |
|<span data-ttu-id="7ee95-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ee95-114">Application</span></span>                            | <span data-ttu-id="7ee95-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ee95-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ee95-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ee95-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="7ee95-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ee95-117">Request headers</span></span>
| <span data-ttu-id="7ee95-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7ee95-118">Name</span></span>         | <span data-ttu-id="7ee95-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7ee95-119">Type</span></span>        | <span data-ttu-id="7ee95-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7ee95-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7ee95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ee95-121">Authorization</span></span> | <span data-ttu-id="7ee95-122">string</span><span class="sxs-lookup"><span data-stu-id="7ee95-122">string</span></span> | <span data-ttu-id="7ee95-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ee95-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ee95-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ee95-125">Request body</span></span>
<span data-ttu-id="7ee95-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ee95-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7ee95-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ee95-127">Response</span></span>
<span data-ttu-id="7ee95-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ee95-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ee95-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7ee95-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ee95-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ee95-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="7ee95-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ee95-132">Response</span></span>
><span data-ttu-id="7ee95-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ee95-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7ee95-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7ee95-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7ee95-136">Языках</span><span class="sxs-lookup"><span data-stu-id="7ee95-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ee95-137">Язык</span><span class="sxs-lookup"><span data-stu-id="7ee95-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_agreement-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
