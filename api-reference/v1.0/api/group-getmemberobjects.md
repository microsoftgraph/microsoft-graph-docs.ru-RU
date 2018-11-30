---
title: 'group: getMemberObjects'
description: Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.
ms.openlocfilehash: 59f3408434c77290552080b6b7b99a20e6fe19db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026531"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="f1d2e-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="f1d2e-105">group: getMemberObjects</span></span>
<span data-ttu-id="f1d2e-p102">Возврат всех групп, в которых состоит эта группа. Это транзитивная проверка. Примечание. Группы не могут быть членами ролей каталога, поэтому роли каталогов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1d2e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d2e-109">Permissions</span></span>
<span data-ttu-id="f1d2e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d2e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d2e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d2e-112">Permission type</span></span>      | <span data-ttu-id="f1d2e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1d2e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1d2e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1d2e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f1d2e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1d2e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1d2e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1d2e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1d2e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-117">Not supported.</span></span>    |
|<span data-ttu-id="f1d2e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1d2e-118">Application</span></span> | <span data-ttu-id="f1d2e-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d2e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1d2e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1d2e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="f1d2e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1d2e-121">Request headers</span></span>
| <span data-ttu-id="f1d2e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f1d2e-122">Name</span></span>       | <span data-ttu-id="f1d2e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f1d2e-123">Type</span></span> | <span data-ttu-id="f1d2e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f1d2e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1d2e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1d2e-125">Authorization</span></span>  | <span data-ttu-id="f1d2e-126">string</span><span class="sxs-lookup"><span data-stu-id="f1d2e-126">string</span></span>  | <span data-ttu-id="f1d2e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1d2e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1d2e-129">Request body</span></span>
<span data-ttu-id="f1d2e-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f1d2e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f1d2e-131">Parameter</span></span>    | <span data-ttu-id="f1d2e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f1d2e-132">Type</span></span>   |<span data-ttu-id="f1d2e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f1d2e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1d2e-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f1d2e-134">securityEnabledOnly</span></span>|<span data-ttu-id="f1d2e-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="f1d2e-135">Boolean</span></span>| <span data-ttu-id="f1d2e-p105">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="f1d2e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1d2e-138">Response</span></span>
<span data-ttu-id="f1d2e-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="f1d2e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f1d2e-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f1d2e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1d2e-141">Request</span></span>
<span data-ttu-id="f1d2e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="f1d2e-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1d2e-143">Response</span></span>
<span data-ttu-id="f1d2e-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-144">The following is an example of the response.</span></span>
><span data-ttu-id="f1d2e-145">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f1d2e-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1d2e-146">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
