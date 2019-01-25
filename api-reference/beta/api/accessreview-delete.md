---
title: Удаление accessReview
description: Доступ к функции проверки в Azure AD, удалить объект accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28848cc047306259248d0ba4663ab3eb3e964224
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527775"
---
# <a name="delete-accessreview"></a><span data-ttu-id="6e8bc-103">Удаление accessReview</span><span class="sxs-lookup"><span data-stu-id="6e8bc-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e8bc-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD удалите объект [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="6e8bc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e8bc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8bc-105">Permissions</span></span>
<span data-ttu-id="6e8bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e8bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e8bc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8bc-108">Permission type</span></span>                        | <span data-ttu-id="6e8bc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e8bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e8bc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e8bc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e8bc-111">AccessReview.ReadWrite.All, а также должны иметь ProgramControl.ReadWrite.All для выполнения сценария с помощью вызова для удаления programControl</span><span class="sxs-lookup"><span data-stu-id="6e8bc-111">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="6e8bc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e8bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e8bc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8bc-113">Not supported.</span></span> |
|<span data-ttu-id="6e8bc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e8bc-114">Application</span></span>                            | <span data-ttu-id="6e8bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e8bc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e8bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="6e8bc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e8bc-117">Request headers</span></span>
| <span data-ttu-id="6e8bc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6e8bc-118">Name</span></span>         | <span data-ttu-id="6e8bc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6e8bc-119">Type</span></span>        | <span data-ttu-id="6e8bc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6e8bc-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6e8bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e8bc-121">Authorization</span></span> | <span data-ttu-id="6e8bc-122">string</span><span class="sxs-lookup"><span data-stu-id="6e8bc-122">string</span></span> | <span data-ttu-id="6e8bc-123">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="6e8bc-123">Bearer \{token\}.</span></span> <span data-ttu-id="6e8bc-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e8bc-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e8bc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e8bc-125">Request body</span></span>
<span data-ttu-id="6e8bc-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e8bc-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6e8bc-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e8bc-127">Response</span></span>
<span data-ttu-id="6e8bc-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e8bc-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e8bc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6e8bc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e8bc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e8bc-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="6e8bc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e8bc-132">Response</span></span>
><span data-ttu-id="6e8bc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e8bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
