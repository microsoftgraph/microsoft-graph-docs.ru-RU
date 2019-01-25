---
title: 'NamedItem: Range'
description: Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.
localization_priority: Normal
ms.openlocfilehash: 283eadbe423fad415534bb4e355f7926e24628be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517682"
---
# <a name="nameditem-range"></a><span data-ttu-id="f14d9-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="f14d9-104">NamedItem: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f14d9-p102">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="f14d9-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f14d9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f14d9-107">Permissions</span></span>
<span data-ttu-id="f14d9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f14d9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f14d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f14d9-110">Permission type</span></span>      | <span data-ttu-id="f14d9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f14d9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f14d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f14d9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f14d9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f14d9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f14d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f14d9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f14d9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f14d9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f14d9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f14d9-116">Application</span></span> | <span data-ttu-id="f14d9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f14d9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f14d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f14d9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/Range

```
## <a name="request-headers"></a><span data-ttu-id="f14d9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f14d9-119">Request headers</span></span>
| <span data-ttu-id="f14d9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f14d9-120">Name</span></span>       | <span data-ttu-id="f14d9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f14d9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f14d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f14d9-122">Authorization</span></span>  | <span data-ttu-id="f14d9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f14d9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f14d9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f14d9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f14d9-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f14d9-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f14d9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f14d9-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f14d9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f14d9-129">Response</span></span>

<span data-ttu-id="f14d9-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f14d9-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f14d9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f14d9-131">Example</span></span>
<span data-ttu-id="f14d9-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f14d9-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f14d9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f14d9-133">Request</span></span>
<span data-ttu-id="f14d9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f14d9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/Range
```

##### <a name="response"></a><span data-ttu-id="f14d9-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="f14d9-135">Response</span></span>
<span data-ttu-id="f14d9-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f14d9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
