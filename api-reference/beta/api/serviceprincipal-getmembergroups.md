---
title: 'servicePrincipal: getMemberGroups'
description: Получение списка групп, участника-службы является членом.  Проверка доверия транзитивных.
localization_priority: Normal
ms.openlocfilehash: 80d81444b9e70bd27b5bc5346ffa0e42e9371837
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519642"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="5a20d-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5a20d-104">servicePrincipal: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a20d-105">Получение списка групп, участника-службы является членом.</span><span class="sxs-lookup"><span data-stu-id="5a20d-105">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="5a20d-106">Проверка доверия транзитивных.</span><span class="sxs-lookup"><span data-stu-id="5a20d-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a20d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a20d-107">Permissions</span></span>
<span data-ttu-id="5a20d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a20d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5a20d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a20d-110">Permission type</span></span>      | <span data-ttu-id="5a20d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a20d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a20d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a20d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a20d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a20d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a20d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a20d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a20d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a20d-115">Not supported.</span></span>    |
|<span data-ttu-id="5a20d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a20d-116">Application</span></span> | <span data-ttu-id="5a20d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a20d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a20d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a20d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="5a20d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a20d-119">Request headers</span></span>
| <span data-ttu-id="5a20d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5a20d-120">Name</span></span>       | <span data-ttu-id="5a20d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5a20d-121">Type</span></span> | <span data-ttu-id="5a20d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a20d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a20d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a20d-123">Authorization</span></span>  | <span data-ttu-id="5a20d-124">string</span><span class="sxs-lookup"><span data-stu-id="5a20d-124">string</span></span>  | <span data-ttu-id="5a20d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a20d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a20d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a20d-127">Request body</span></span>
<span data-ttu-id="5a20d-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5a20d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a20d-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="5a20d-129">Parameter</span></span>    | <span data-ttu-id="5a20d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5a20d-130">Type</span></span>   |<span data-ttu-id="5a20d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5a20d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a20d-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5a20d-132">securityEnabledOnly</span></span>|<span data-ttu-id="5a20d-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="5a20d-133">Boolean</span></span>|<span data-ttu-id="5a20d-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="5a20d-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="5a20d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a20d-136">Response</span></span>

<span data-ttu-id="5a20d-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a20d-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a20d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5a20d-138">Example</span></span>
<span data-ttu-id="5a20d-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5a20d-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5a20d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a20d-140">Request</span></span>
<span data-ttu-id="5a20d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a20d-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5a20d-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a20d-142">Response</span></span>
<span data-ttu-id="5a20d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5a20d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-getmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
