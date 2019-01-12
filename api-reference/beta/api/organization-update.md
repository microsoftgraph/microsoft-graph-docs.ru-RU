---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ed49dcd0546fedf16572bcf75a8c4366395f1fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964440"
---
# <a name="update-organization"></a><span data-ttu-id="a0642-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="a0642-103">Update organization</span></span>

> <span data-ttu-id="a0642-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0642-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0642-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0642-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0642-106">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="a0642-106">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="a0642-107">В этом случае `organization` представляет собой коллекцию только одну запись, поэтому его **идентификатор** должен быть указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="a0642-107">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="a0642-108">**Идентификатор** также называется **tenantId** организации.</span><span class="sxs-lookup"><span data-stu-id="a0642-108">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0642-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0642-109">Permissions</span></span>

<span data-ttu-id="a0642-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0642-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0642-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0642-112">Permission type</span></span> | <span data-ttu-id="a0642-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0642-113">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0642-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0642-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a0642-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0642-115">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a0642-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0642-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0642-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0642-117">Not supported.</span></span> |
|<span data-ttu-id="a0642-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0642-118">Application</span></span> | <span data-ttu-id="a0642-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0642-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0642-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0642-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a0642-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0642-121">Request headers</span></span>

| <span data-ttu-id="a0642-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a0642-122">Name</span></span>       | <span data-ttu-id="a0642-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a0642-123">Type</span></span> | <span data-ttu-id="a0642-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a0642-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a0642-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0642-125">Authorization</span></span>  | <span data-ttu-id="a0642-126">строка</span><span class="sxs-lookup"><span data-stu-id="a0642-126">string</span></span>  | <span data-ttu-id="a0642-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0642-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0642-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0642-129">Request body</span></span>

<span data-ttu-id="a0642-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a0642-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a0642-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0642-133">Property</span></span>     | <span data-ttu-id="a0642-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a0642-134">Type</span></span>   |<span data-ttu-id="a0642-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a0642-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0642-136">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a0642-136">marketingNotificationEmails</span></span>|<span data-ttu-id="a0642-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0642-137">String collection</span></span>|                                        <span data-ttu-id="a0642-138">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="a0642-138">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="a0642-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="a0642-139">privacyProfile</span></span>|[<span data-ttu-id="a0642-140">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="a0642-140">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="a0642-141">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="a0642-141">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="a0642-142">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="a0642-142">securityComplianceNotificationMails</span></span>|<span data-ttu-id="a0642-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0642-143">String collection</span></span>||
|<span data-ttu-id="a0642-144">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="a0642-144">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="a0642-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0642-145">String collection</span></span>||
|<span data-ttu-id="a0642-146">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="a0642-146">technicalNotificationMails</span></span>|<span data-ttu-id="a0642-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0642-147">String collection</span></span>|                                        <span data-ttu-id="a0642-148">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="a0642-148">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="a0642-149">Поскольку ресурсов **организации** поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **организации** .</span><span class="sxs-lookup"><span data-stu-id="a0642-149">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="a0642-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0642-150">Response</span></span>

<span data-ttu-id="a0642-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a0642-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0642-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a0642-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0642-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0642-154">Request</span></span>
<span data-ttu-id="a0642-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0642-155">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a0642-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0642-156">Response</span></span>

<span data-ttu-id="a0642-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a0642-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a0642-158">См. также</span><span class="sxs-lookup"><span data-stu-id="a0642-158">See also</span></span>

- [<span data-ttu-id="a0642-159">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a0642-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a0642-160">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a0642-160">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
