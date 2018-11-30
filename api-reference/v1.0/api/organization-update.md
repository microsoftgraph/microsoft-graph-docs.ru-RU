---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
ms.openlocfilehash: ac07f3ded31f8d6c7169d24208ed7e8cf967e07a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027581"
---
# <a name="update-organization"></a><span data-ttu-id="4444a-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="4444a-103">Update organization</span></span>

<span data-ttu-id="4444a-104">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="4444a-104">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="4444a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4444a-105">Permissions</span></span>

<span data-ttu-id="4444a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4444a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4444a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4444a-108">Permission type</span></span> | <span data-ttu-id="4444a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4444a-109">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4444a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4444a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4444a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4444a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4444a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4444a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4444a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4444a-113">Not supported.</span></span>    |
|<span data-ttu-id="4444a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4444a-114">Application</span></span> | <span data-ttu-id="4444a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4444a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4444a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4444a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="4444a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4444a-117">Request headers</span></span>

| <span data-ttu-id="4444a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4444a-118">Name</span></span>       | <span data-ttu-id="4444a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4444a-119">Type</span></span> | <span data-ttu-id="4444a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4444a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4444a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4444a-121">Authorization</span></span>  | <span data-ttu-id="4444a-122">string</span><span class="sxs-lookup"><span data-stu-id="4444a-122">string</span></span>  | <span data-ttu-id="4444a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4444a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4444a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4444a-125">Request body</span></span>
<span data-ttu-id="4444a-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4444a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4444a-127">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4444a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4444a-128">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4444a-128">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4444a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4444a-129">Property</span></span>     | <span data-ttu-id="4444a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4444a-130">Type</span></span>   |<span data-ttu-id="4444a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4444a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4444a-132">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="4444a-132">marketingNotificationEmails</span></span>|<span data-ttu-id="4444a-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4444a-133">String collection</span></span>|                                        <span data-ttu-id="4444a-134">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4444a-134">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4444a-135">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="4444a-135">privacyProfile</span></span>|[<span data-ttu-id="4444a-136">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="4444a-136">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="4444a-137">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="4444a-137">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="4444a-138">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="4444a-138">securityComplianceNotificationMails</span></span>|<span data-ttu-id="4444a-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4444a-139">String collection</span></span>||
|<span data-ttu-id="4444a-140">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="4444a-140">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="4444a-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4444a-141">String collection</span></span>||
|<span data-ttu-id="4444a-142">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="4444a-142">technicalNotificationMails</span></span>|<span data-ttu-id="4444a-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4444a-143">String collection</span></span>|                                        <span data-ttu-id="4444a-144">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4444a-144">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="4444a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4444a-145">Response</span></span>

<span data-ttu-id="4444a-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4444a-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4444a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4444a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4444a-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4444a-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
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

### <a name="response"></a><span data-ttu-id="4444a-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="4444a-149">Response</span></span>

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
