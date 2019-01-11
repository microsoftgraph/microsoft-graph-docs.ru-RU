---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
ms.openlocfilehash: ae91b0f7cf92619f07f042c515bad2aab0d1035a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890421"
---
# <a name="update-organization"></a><span data-ttu-id="4b419-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="4b419-103">Update organization</span></span>

> <span data-ttu-id="4b419-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b419-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b419-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b419-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b419-106">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="4b419-106">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="4b419-107">В этом случае `organization` представляет собой коллекцию только одну запись, поэтому его **идентификатор** должен быть указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="4b419-107">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="4b419-108">**Идентификатор** также называется **tenantId** организации.</span><span class="sxs-lookup"><span data-stu-id="4b419-108">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b419-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b419-109">Permissions</span></span>

<span data-ttu-id="4b419-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b419-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b419-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b419-112">Permission type</span></span> | <span data-ttu-id="4b419-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b419-113">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b419-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b419-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4b419-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b419-115">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4b419-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b419-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b419-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b419-117">Not supported.</span></span> |
|<span data-ttu-id="4b419-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b419-118">Application</span></span> | <span data-ttu-id="4b419-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b419-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b419-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b419-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b419-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b419-121">Request headers</span></span>

| <span data-ttu-id="4b419-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4b419-122">Name</span></span>       | <span data-ttu-id="4b419-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4b419-123">Type</span></span> | <span data-ttu-id="4b419-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4b419-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b419-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b419-125">Authorization</span></span>  | <span data-ttu-id="4b419-126">string</span><span class="sxs-lookup"><span data-stu-id="4b419-126">string</span></span>  | <span data-ttu-id="4b419-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b419-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b419-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b419-129">Request body</span></span>

<span data-ttu-id="4b419-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4b419-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b419-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b419-133">Property</span></span>     | <span data-ttu-id="4b419-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4b419-134">Type</span></span>   |<span data-ttu-id="4b419-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4b419-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b419-136">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="4b419-136">marketingNotificationEmails</span></span>|<span data-ttu-id="4b419-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b419-137">String collection</span></span>|                                        <span data-ttu-id="4b419-138">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4b419-138">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="4b419-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="4b419-139">privacyProfile</span></span>|[<span data-ttu-id="4b419-140">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="4b419-140">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="4b419-141">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="4b419-141">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="4b419-142">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="4b419-142">securityComplianceNotificationMails</span></span>|<span data-ttu-id="4b419-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b419-143">String collection</span></span>||
|<span data-ttu-id="4b419-144">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="4b419-144">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="4b419-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b419-145">String collection</span></span>||
|<span data-ttu-id="4b419-146">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="4b419-146">technicalNotificationMails</span></span>|<span data-ttu-id="4b419-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b419-147">String collection</span></span>|                                        <span data-ttu-id="4b419-148">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="4b419-148">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="4b419-149">Поскольку ресурсов **организации** поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **организации** .</span><span class="sxs-lookup"><span data-stu-id="4b419-149">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="4b419-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b419-150">Response</span></span>

<span data-ttu-id="4b419-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4b419-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b419-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4b419-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b419-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b419-154">Request</span></span>
<span data-ttu-id="4b419-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b419-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
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

##### <a name="response"></a><span data-ttu-id="4b419-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b419-156">Response</span></span>

<span data-ttu-id="4b419-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b419-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4b419-158">См. также</span><span class="sxs-lookup"><span data-stu-id="4b419-158">See also</span></span>

- [<span data-ttu-id="4b419-159">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4b419-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4b419-160">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4b419-160">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
