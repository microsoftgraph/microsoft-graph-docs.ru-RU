---
title: Вывод групп элементов
description: Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1d0bb1af8e88c125a0f4a672c431a21e1f5d9c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571970"
---
# <a name="get-member-groups"></a><span data-ttu-id="8c702-104">Вывод групп элементов</span><span class="sxs-lookup"><span data-stu-id="8c702-104">Get member groups</span></span>

<span data-ttu-id="8c702-p102">Возвращает все группы, в которых состоит указанный пользователь, группа или объект каталога. Это транзитивная функция.</span><span class="sxs-lookup"><span data-stu-id="8c702-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c702-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c702-107">Permissions</span></span>
<span data-ttu-id="8c702-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c702-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c702-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c702-110">Permission type</span></span>      | <span data-ttu-id="8c702-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c702-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c702-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c702-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c702-113">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c702-113">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="8c702-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c702-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c702-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c702-115">Not supported.</span></span>    |
|<span data-ttu-id="8c702-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c702-116">Application</span></span> | <span data-ttu-id="8c702-117">User.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c702-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c702-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c702-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="8c702-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c702-119">Request headers</span></span>
| <span data-ttu-id="8c702-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8c702-120">Name</span></span>       | <span data-ttu-id="8c702-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8c702-121">Type</span></span> | <span data-ttu-id="8c702-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8c702-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c702-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c702-123">Authorization</span></span>  | <span data-ttu-id="8c702-124">string</span><span class="sxs-lookup"><span data-stu-id="8c702-124">string</span></span>  | <span data-ttu-id="8c702-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c702-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c702-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c702-127">Content-Type</span></span>   | <span data-ttu-id="8c702-128">string</span><span class="sxs-lookup"><span data-stu-id="8c702-128">string</span></span>  | <span data-ttu-id="8c702-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8c702-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c702-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c702-130">Request body</span></span>
<span data-ttu-id="8c702-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8c702-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c702-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="8c702-132">Parameter</span></span>    | <span data-ttu-id="8c702-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8c702-133">Type</span></span>   |<span data-ttu-id="8c702-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8c702-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c702-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="8c702-135">securityEnabledOnly</span></span>|<span data-ttu-id="8c702-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="8c702-136">Boolean</span></span>| <span data-ttu-id="8c702-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит объект. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является объект. **Примечание**. Вызвать функцию для пользователя можно, только если для параметра задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="8c702-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="8c702-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c702-139">Response</span></span>

<span data-ttu-id="8c702-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c702-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c702-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8c702-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8c702-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c702-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="8c702-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c702-143">Response</span></span>
<span data-ttu-id="8c702-p106">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c702-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
