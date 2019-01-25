---
title: Удаление соглашения
description: Удаление объекта соглашения.
localization_priority: Normal
ms.openlocfilehash: 95766f28e5456c1b4f410de65ae12dccd881727e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521322"
---
# <a name="delete-agreement"></a><span data-ttu-id="720b8-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="720b8-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="720b8-104">Удаление объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="720b8-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="720b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="720b8-105">Permissions</span></span>
<span data-ttu-id="720b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="720b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="720b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="720b8-108">Permission type</span></span>                        | <span data-ttu-id="720b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="720b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="720b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="720b8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="720b8-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="720b8-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="720b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="720b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="720b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720b8-113">Not supported.</span></span> |
|<span data-ttu-id="720b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="720b8-114">Application</span></span>                            | <span data-ttu-id="720b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720b8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="720b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="720b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="720b8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="720b8-117">Request headers</span></span>
| <span data-ttu-id="720b8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="720b8-118">Name</span></span>         | <span data-ttu-id="720b8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="720b8-119">Type</span></span>        | <span data-ttu-id="720b8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="720b8-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="720b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="720b8-121">Authorization</span></span> | <span data-ttu-id="720b8-122">string</span><span class="sxs-lookup"><span data-stu-id="720b8-122">string</span></span> | <span data-ttu-id="720b8-123">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="720b8-123">Bearer \{token\}.</span></span> <span data-ttu-id="720b8-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="720b8-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="720b8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="720b8-125">Request body</span></span>
<span data-ttu-id="720b8-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="720b8-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="720b8-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="720b8-127">Response</span></span>
<span data-ttu-id="720b8-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="720b8-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="720b8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="720b8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="720b8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="720b8-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="720b8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="720b8-132">Response</span></span>
><span data-ttu-id="720b8-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="720b8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
