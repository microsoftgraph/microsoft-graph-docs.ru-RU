---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 109c3f68e1eaa719f18a7fa8c539d09a2e3061aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969851"
---
# <a name="update-organization"></a><span data-ttu-id="a19d6-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="a19d6-103">Update organization</span></span>

<span data-ttu-id="a19d6-104">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="a19d6-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="a19d6-105">В этом случае `organization` представляет собой коллекцию только одну запись, поэтому его **идентификатор** должен быть указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="a19d6-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="a19d6-106">**Идентификатор** также называется **tenantId** организации.</span><span class="sxs-lookup"><span data-stu-id="a19d6-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="a19d6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a19d6-107">Permissions</span></span>

<span data-ttu-id="a19d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a19d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a19d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a19d6-110">Permission type</span></span> | <span data-ttu-id="a19d6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a19d6-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a19d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a19d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a19d6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a19d6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a19d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a19d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a19d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a19d6-115">Not supported.</span></span>    |
|<span data-ttu-id="a19d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a19d6-116">Application</span></span> | <span data-ttu-id="a19d6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a19d6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a19d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a19d6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="a19d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a19d6-119">Request headers</span></span>

| <span data-ttu-id="a19d6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a19d6-120">Name</span></span>       | <span data-ttu-id="a19d6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a19d6-121">Type</span></span> | <span data-ttu-id="a19d6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a19d6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a19d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a19d6-123">Authorization</span></span>  | <span data-ttu-id="a19d6-124">string</span><span class="sxs-lookup"><span data-stu-id="a19d6-124">string</span></span>  | <span data-ttu-id="a19d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a19d6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a19d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a19d6-127">Request body</span></span>

<span data-ttu-id="a19d6-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a19d6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a19d6-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a19d6-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a19d6-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a19d6-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a19d6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a19d6-131">Property</span></span>     | <span data-ttu-id="a19d6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a19d6-132">Type</span></span>   |<span data-ttu-id="a19d6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a19d6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a19d6-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a19d6-134">marketingNotificationEmails</span></span>|<span data-ttu-id="a19d6-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a19d6-135">String collection</span></span>|                                        <span data-ttu-id="a19d6-136">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="a19d6-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="a19d6-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="a19d6-137">privacyProfile</span></span>|[<span data-ttu-id="a19d6-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="a19d6-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="a19d6-139">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="a19d6-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="a19d6-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="a19d6-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="a19d6-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a19d6-141">String collection</span></span>||
|<span data-ttu-id="a19d6-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="a19d6-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="a19d6-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a19d6-143">String collection</span></span>||
|<span data-ttu-id="a19d6-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="a19d6-144">technicalNotificationMails</span></span>|<span data-ttu-id="a19d6-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a19d6-145">String collection</span></span>|                                        <span data-ttu-id="a19d6-146">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="a19d6-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="a19d6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a19d6-147">Response</span></span>

<span data-ttu-id="a19d6-148">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a19d6-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a19d6-149">Пример</span><span class="sxs-lookup"><span data-stu-id="a19d6-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a19d6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a19d6-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="a19d6-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="a19d6-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
