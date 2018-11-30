---
title: Вывод объектов элементов
description: " Возвращает все группы, административные единиц измерения и каталог роли, которые пользователь, группа, субъектов-служб или объекта directory является членом. Эта функция транзитивное. "
ms.openlocfilehash: f1bf68276fc4ed7d4694fadc73a08ae328047222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074994"
---
# <a name="get-member-objects"></a><span data-ttu-id="2123a-104">Вывод объектов элементов</span><span class="sxs-lookup"><span data-stu-id="2123a-104">Get member objects</span></span>

> <span data-ttu-id="2123a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2123a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2123a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2123a-106">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="2123a-107">Возвращает все группы, административные единиц измерения и каталог роли, которые пользователь, группа, субъектов-служб или объекта directory является членом.</span><span class="sxs-lookup"><span data-stu-id="2123a-107">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="2123a-108">Эта функция транзитивное.</span><span class="sxs-lookup"><span data-stu-id="2123a-108">This function is transitive.</span></span> 
 > <span data-ttu-id="2123a-109">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="2123a-109">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="2123a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2123a-110">Permissions</span></span>
<span data-ttu-id="2123a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2123a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2123a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2123a-113">Permission type</span></span>      | <span data-ttu-id="2123a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2123a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2123a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2123a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2123a-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2123a-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="2123a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2123a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2123a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2123a-118">Not supported.</span></span>    |
|<span data-ttu-id="2123a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2123a-119">Application</span></span> | <span data-ttu-id="2123a-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2123a-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2123a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2123a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="2123a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2123a-122">Request headers</span></span>
| <span data-ttu-id="2123a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2123a-123">Name</span></span>       | <span data-ttu-id="2123a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="2123a-124">Type</span></span> | <span data-ttu-id="2123a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2123a-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2123a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2123a-126">Authorization</span></span>  | <span data-ttu-id="2123a-127">string</span><span class="sxs-lookup"><span data-stu-id="2123a-127">string</span></span>  | <span data-ttu-id="2123a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2123a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2123a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2123a-130">Content-Type</span></span>  | <span data-ttu-id="2123a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2123a-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2123a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2123a-132">Request body</span></span>
<span data-ttu-id="2123a-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2123a-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2123a-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="2123a-134">Parameter</span></span>    | <span data-ttu-id="2123a-135">Тип</span><span class="sxs-lookup"><span data-stu-id="2123a-135">Type</span></span>   |<span data-ttu-id="2123a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="2123a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2123a-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2123a-137">securityEnabledOnly</span></span>|<span data-ttu-id="2123a-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="2123a-138">Boolean</span></span>| <span data-ttu-id="2123a-p106">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="2123a-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="2123a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2123a-141">Response</span></span>

<span data-ttu-id="2123a-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2123a-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2123a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2123a-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2123a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2123a-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="2123a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2123a-145">Response</span></span>
<span data-ttu-id="2123a-p107">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2123a-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
