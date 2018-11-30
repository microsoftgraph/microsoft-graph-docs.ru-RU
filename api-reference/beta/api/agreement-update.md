---
title: Обновить соглашения
description: Обновляет свойства объекта соглашения.
ms.openlocfilehash: b9405a8c469876a349b5c1b0c00e6f6a5f225e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075745"
---
# <a name="update-agreement"></a><span data-ttu-id="44771-103">Обновить соглашения</span><span class="sxs-lookup"><span data-stu-id="44771-103">Update agreement</span></span>

> <span data-ttu-id="44771-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44771-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44771-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44771-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44771-106">Обновляет свойства объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="44771-106">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="44771-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44771-107">Permissions</span></span>
<span data-ttu-id="44771-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44771-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44771-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44771-110">Permission type</span></span>                        | <span data-ttu-id="44771-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44771-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="44771-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44771-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="44771-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44771-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="44771-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44771-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44771-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44771-115">Not supported.</span></span> |
|<span data-ttu-id="44771-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44771-116">Application</span></span>                            | <span data-ttu-id="44771-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44771-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44771-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44771-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="44771-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44771-119">Request headers</span></span>
| <span data-ttu-id="44771-120">Имя</span><span class="sxs-lookup"><span data-stu-id="44771-120">Name</span></span>         | <span data-ttu-id="44771-121">Тип</span><span class="sxs-lookup"><span data-stu-id="44771-121">Type</span></span>        | <span data-ttu-id="44771-122">Описание</span><span class="sxs-lookup"><span data-stu-id="44771-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="44771-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44771-123">Authorization</span></span> | <span data-ttu-id="44771-124">string</span><span class="sxs-lookup"><span data-stu-id="44771-124">string</span></span> | <span data-ttu-id="44771-125">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="44771-125">Bearer \{token\}.</span></span> <span data-ttu-id="44771-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="44771-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44771-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44771-127">Request body</span></span>
<span data-ttu-id="44771-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="44771-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="44771-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="44771-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="44771-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="44771-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44771-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="44771-131">Property</span></span>     | <span data-ttu-id="44771-132">Тип</span><span class="sxs-lookup"><span data-stu-id="44771-132">Type</span></span>        | <span data-ttu-id="44771-133">Описание</span><span class="sxs-lookup"><span data-stu-id="44771-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44771-134">displayName</span><span class="sxs-lookup"><span data-stu-id="44771-134">displayName</span></span>|<span data-ttu-id="44771-135">String</span><span class="sxs-lookup"><span data-stu-id="44771-135">String</span></span>|<span data-ttu-id="44771-136">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="44771-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="44771-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="44771-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="44771-138">Логический</span><span class="sxs-lookup"><span data-stu-id="44771-138">Boolean</span></span>|<span data-ttu-id="44771-139">Имеет ли пользователь можно развернуть и отобразить соглашения перед подтверждением.</span><span class="sxs-lookup"><span data-stu-id="44771-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="44771-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="44771-140">Response</span></span>
<span data-ttu-id="44771-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект обновленные [соглашения](../resources/agreement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44771-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="44771-142">Пример</span><span class="sxs-lookup"><span data-stu-id="44771-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44771-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="44771-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="44771-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="44771-144">Response</span></span>
><span data-ttu-id="44771-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44771-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
