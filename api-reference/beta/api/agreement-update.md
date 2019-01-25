---
title: Обновить соглашения
description: Обновляет свойства объекта соглашения.
localization_priority: Normal
ms.openlocfilehash: fc6e4718a026f78a6e892dc13095492099b654cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520069"
---
# <a name="update-agreement"></a><span data-ttu-id="79992-103">Обновить соглашения</span><span class="sxs-lookup"><span data-stu-id="79992-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79992-104">Обновляет свойства объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="79992-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="79992-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79992-105">Permissions</span></span>
<span data-ttu-id="79992-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79992-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79992-108">Permission type</span></span>                        | <span data-ttu-id="79992-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79992-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="79992-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79992-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79992-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79992-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="79992-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79992-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79992-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79992-113">Not supported.</span></span> |
|<span data-ttu-id="79992-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79992-114">Application</span></span>                            | <span data-ttu-id="79992-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79992-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79992-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79992-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="79992-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79992-117">Request headers</span></span>
| <span data-ttu-id="79992-118">Имя</span><span class="sxs-lookup"><span data-stu-id="79992-118">Name</span></span>         | <span data-ttu-id="79992-119">Тип</span><span class="sxs-lookup"><span data-stu-id="79992-119">Type</span></span>        | <span data-ttu-id="79992-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79992-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="79992-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79992-121">Authorization</span></span> | <span data-ttu-id="79992-122">string</span><span class="sxs-lookup"><span data-stu-id="79992-122">string</span></span> | <span data-ttu-id="79992-123">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="79992-123">Bearer \{token\}.</span></span> <span data-ttu-id="79992-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79992-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79992-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79992-125">Request body</span></span>
<span data-ttu-id="79992-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="79992-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="79992-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="79992-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="79992-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="79992-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79992-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="79992-129">Property</span></span>     | <span data-ttu-id="79992-130">Тип</span><span class="sxs-lookup"><span data-stu-id="79992-130">Type</span></span>        | <span data-ttu-id="79992-131">Описание</span><span class="sxs-lookup"><span data-stu-id="79992-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79992-132">displayName</span><span class="sxs-lookup"><span data-stu-id="79992-132">displayName</span></span>|<span data-ttu-id="79992-133">String</span><span class="sxs-lookup"><span data-stu-id="79992-133">String</span></span>|<span data-ttu-id="79992-134">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="79992-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="79992-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="79992-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="79992-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="79992-136">Boolean</span></span>|<span data-ttu-id="79992-137">Имеет ли пользователь можно развернуть и отобразить соглашения перед подтверждением.</span><span class="sxs-lookup"><span data-stu-id="79992-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="79992-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="79992-138">Response</span></span>
<span data-ttu-id="79992-139">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект обновленные [соглашения](../resources/agreement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="79992-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79992-140">Пример</span><span class="sxs-lookup"><span data-stu-id="79992-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79992-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="79992-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="79992-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="79992-142">Response</span></span>
><span data-ttu-id="79992-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79992-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
