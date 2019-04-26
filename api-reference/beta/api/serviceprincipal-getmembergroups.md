---
title: 'servicePrincipal: getMemberGroups'
description: Получение списка групп, членом которых является данный участник службы.  Это транзитивная проверка.
localization_priority: Normal
ms.openlocfilehash: 6692f9be6ae3f99c82d9f0d9e2bfd30d043f47b2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331508"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="2721f-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2721f-104">servicePrincipal: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2721f-105">Получение списка групп, членом которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="2721f-105">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="2721f-106">Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="2721f-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="2721f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2721f-107">Permissions</span></span>
<span data-ttu-id="2721f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2721f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2721f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2721f-110">Permission type</span></span>      | <span data-ttu-id="2721f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2721f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2721f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2721f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2721f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2721f-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2721f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2721f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2721f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2721f-115">Not supported.</span></span>    |
|<span data-ttu-id="2721f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2721f-116">Application</span></span> | <span data-ttu-id="2721f-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2721f-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2721f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2721f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="2721f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2721f-119">Request headers</span></span>
| <span data-ttu-id="2721f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2721f-120">Name</span></span>       | <span data-ttu-id="2721f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2721f-121">Type</span></span> | <span data-ttu-id="2721f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2721f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2721f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2721f-123">Authorization</span></span>  | <span data-ttu-id="2721f-124">string</span><span class="sxs-lookup"><span data-stu-id="2721f-124">string</span></span>  | <span data-ttu-id="2721f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2721f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2721f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2721f-127">Request body</span></span>
<span data-ttu-id="2721f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2721f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2721f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="2721f-129">Parameter</span></span>    | <span data-ttu-id="2721f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2721f-130">Type</span></span>   |<span data-ttu-id="2721f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2721f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2721f-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2721f-132">securityEnabledOnly</span></span>|<span data-ttu-id="2721f-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="2721f-133">Boolean</span></span>|<span data-ttu-id="2721f-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="2721f-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="2721f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2721f-136">Response</span></span>

<span data-ttu-id="2721f-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2721f-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2721f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2721f-138">Example</span></span>
<span data-ttu-id="2721f-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2721f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2721f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2721f-140">Request</span></span>
<span data-ttu-id="2721f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2721f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="2721f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2721f-142">Response</span></span>
<span data-ttu-id="2721f-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2721f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
