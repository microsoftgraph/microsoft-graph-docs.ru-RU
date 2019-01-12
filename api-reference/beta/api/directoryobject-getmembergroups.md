---
title: Вывод групп элементов
description: Возвращает все группы, что указанный пользователь, группа, участника службы или объект каталога, является участником из. Эта функция транзитивное.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53d52ae4d877f3367fa6b08ea73cefa1fea492cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935866"
---
# <a name="get-member-groups"></a><span data-ttu-id="0fa9b-104">Вывод групп элементов</span><span class="sxs-lookup"><span data-stu-id="0fa9b-104">Get member groups</span></span>

> <span data-ttu-id="0fa9b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fa9b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fa9b-107">Возвращает все группы, что указанный пользователь, группа, участника службы или объект каталога, является участником из.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-107">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="0fa9b-108">Эта функция транзитивное.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-108">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa9b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa9b-109">Permissions</span></span>
<span data-ttu-id="0fa9b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa9b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0fa9b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa9b-112">Permission type</span></span>      | <span data-ttu-id="0fa9b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fa9b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fa9b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fa9b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0fa9b-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fa9b-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="0fa9b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fa9b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa9b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-117">Not supported.</span></span>    |
|<span data-ttu-id="0fa9b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fa9b-118">Application</span></span> | <span data-ttu-id="0fa9b-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0fa9b-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fa9b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fa9b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="0fa9b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fa9b-121">Request headers</span></span>
| <span data-ttu-id="0fa9b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0fa9b-122">Name</span></span>       | <span data-ttu-id="0fa9b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0fa9b-123">Type</span></span> | <span data-ttu-id="0fa9b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa9b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fa9b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa9b-125">Authorization</span></span>  | <span data-ttu-id="0fa9b-126">string</span><span class="sxs-lookup"><span data-stu-id="0fa9b-126">string</span></span>  | <span data-ttu-id="0fa9b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0fa9b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fa9b-129">Content-Type</span></span>  | <span data-ttu-id="0fa9b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="0fa9b-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fa9b-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fa9b-131">Request body</span></span>
<span data-ttu-id="0fa9b-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0fa9b-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="0fa9b-133">Parameter</span></span>    | <span data-ttu-id="0fa9b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0fa9b-134">Type</span></span>   |<span data-ttu-id="0fa9b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa9b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fa9b-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0fa9b-136">securityEnabledOnly</span></span>|<span data-ttu-id="0fa9b-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="0fa9b-137">Boolean</span></span>| <span data-ttu-id="0fa9b-p106">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="0fa9b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa9b-140">Response</span></span>

<span data-ttu-id="0fa9b-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa9b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="0fa9b-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0fa9b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa9b-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="0fa9b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa9b-144">Response</span></span>
<span data-ttu-id="0fa9b-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fa9b-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
