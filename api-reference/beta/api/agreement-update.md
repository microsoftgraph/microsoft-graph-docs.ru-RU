---
title: Обновление соглашения
description: Обновление свойств объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: a134e26f6e2b8d2994d960759d389525a80673e4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471567"
---
# <a name="update-agreement"></a><span data-ttu-id="8751d-103">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="8751d-103">Update agreement</span></span>

<span data-ttu-id="8751d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8751d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8751d-105">Обновление свойств объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="8751d-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8751d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8751d-106">Permissions</span></span>
<span data-ttu-id="8751d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8751d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8751d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8751d-109">Permission type</span></span>                        | <span data-ttu-id="8751d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8751d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8751d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8751d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8751d-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8751d-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="8751d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8751d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8751d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8751d-114">Not supported.</span></span> |
|<span data-ttu-id="8751d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8751d-115">Application</span></span>                            | <span data-ttu-id="8751d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8751d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8751d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8751d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8751d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8751d-118">Request headers</span></span>
| <span data-ttu-id="8751d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8751d-119">Name</span></span>         | <span data-ttu-id="8751d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8751d-120">Type</span></span>        | <span data-ttu-id="8751d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8751d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8751d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8751d-122">Authorization</span></span> | <span data-ttu-id="8751d-123">string</span><span class="sxs-lookup"><span data-stu-id="8751d-123">string</span></span> | <span data-ttu-id="8751d-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8751d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8751d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8751d-126">Request body</span></span>
<span data-ttu-id="8751d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8751d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8751d-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8751d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8751d-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8751d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8751d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8751d-130">Property</span></span>     | <span data-ttu-id="8751d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8751d-131">Type</span></span>        | <span data-ttu-id="8751d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8751d-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8751d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8751d-133">displayName</span></span>|<span data-ttu-id="8751d-134">String</span><span class="sxs-lookup"><span data-stu-id="8751d-134">String</span></span>|<span data-ttu-id="8751d-135">Отображение имени соглашения.</span><span class="sxs-lookup"><span data-stu-id="8751d-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="8751d-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="8751d-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="8751d-137">Логический</span><span class="sxs-lookup"><span data-stu-id="8751d-137">Boolean</span></span>|<span data-ttu-id="8751d-138">Необходимо ли пользователю расширить и просмотреть соглашение перед его принятием.</span><span class="sxs-lookup"><span data-stu-id="8751d-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="8751d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8751d-139">Response</span></span>
<span data-ttu-id="8751d-140">В случае успешной работы этот метод возвращает код отклика и обновленный объект соглашения `200 OK` в тексте [](../resources/agreement.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="8751d-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8751d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8751d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8751d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8751d-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```

##### <a name="response"></a><span data-ttu-id="8751d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8751d-143">Response</span></span>
><span data-ttu-id="8751d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8751d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->


