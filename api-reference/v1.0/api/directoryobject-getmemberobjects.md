---
title: Вывод объектов элементов
description: " Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная функция. "
localization_priority: Normal
ms.openlocfilehash: b7c4c09991d31141e12fb6cd900309f81e22f8e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815913"
---
# <a name="get-member-objects"></a><span data-ttu-id="06572-104">Вывод объектов элементов</span><span class="sxs-lookup"><span data-stu-id="06572-104">Get member objects</span></span>

 <span data-ttu-id="06572-p102">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="06572-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="06572-107">Примечание. Участниками ролей каталога могут быть только пользователи.</span><span class="sxs-lookup"><span data-stu-id="06572-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="06572-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06572-108">Permissions</span></span>
<span data-ttu-id="06572-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06572-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06572-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06572-111">Permission type</span></span>      | <span data-ttu-id="06572-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06572-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06572-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06572-113">Delegated (work or school account)</span></span> | <span data-ttu-id="06572-114">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="06572-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="06572-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06572-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06572-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06572-116">Not supported.</span></span>    |
|<span data-ttu-id="06572-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06572-117">Application</span></span> | <span data-ttu-id="06572-118">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="06572-118">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06572-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06572-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="06572-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06572-120">Request headers</span></span>
| <span data-ttu-id="06572-121">Имя</span><span class="sxs-lookup"><span data-stu-id="06572-121">Name</span></span>       | <span data-ttu-id="06572-122">Тип</span><span class="sxs-lookup"><span data-stu-id="06572-122">Type</span></span> | <span data-ttu-id="06572-123">Описание</span><span class="sxs-lookup"><span data-stu-id="06572-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="06572-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="06572-124">Authorization</span></span>  | <span data-ttu-id="06572-125">string</span><span class="sxs-lookup"><span data-stu-id="06572-125">string</span></span>  | <span data-ttu-id="06572-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06572-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06572-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06572-128">Content-Type</span></span>   | <span data-ttu-id="06572-129">строка</span><span class="sxs-lookup"><span data-stu-id="06572-129">string</span></span>  | <span data-ttu-id="06572-130">application/json</span><span class="sxs-lookup"><span data-stu-id="06572-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06572-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06572-131">Request body</span></span>
<span data-ttu-id="06572-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="06572-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06572-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="06572-133">Parameter</span></span>    | <span data-ttu-id="06572-134">Тип</span><span class="sxs-lookup"><span data-stu-id="06572-134">Type</span></span>   |<span data-ttu-id="06572-135">Описание</span><span class="sxs-lookup"><span data-stu-id="06572-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06572-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="06572-136">securityEnabledOnly</span></span>|<span data-ttu-id="06572-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="06572-137">Boolean</span></span>| <span data-ttu-id="06572-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="06572-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="06572-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="06572-140">Response</span></span>

<span data-ttu-id="06572-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06572-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06572-142">Пример</span><span class="sxs-lookup"><span data-stu-id="06572-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="06572-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="06572-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="06572-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="06572-144">Response</span></span>
<span data-ttu-id="06572-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06572-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
