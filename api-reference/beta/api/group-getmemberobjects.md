---
title: 'group: getMemberObjects'
description: 'Возвращает все группы и административных единиц измерения, которые должна быть членом группы. Проверка доверия транзитивных. Примечание: Группы не может быть члены роли каталога, поэтому роли не каталог не возвращается.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a83987a15f384cf17e268a8bdbd6791164484f7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935929"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="04ab5-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="04ab5-105">group: getMemberObjects</span></span>

> <span data-ttu-id="04ab5-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04ab5-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04ab5-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04ab5-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04ab5-108">Возвращает все группы и административных единиц измерения, которые должна быть членом группы.</span><span class="sxs-lookup"><span data-stu-id="04ab5-108">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="04ab5-109">Проверка доверия транзитивных.</span><span class="sxs-lookup"><span data-stu-id="04ab5-109">The check is transitive.</span></span> <span data-ttu-id="04ab5-110">Примечание: Группы не может быть члены роли каталога, поэтому роли не каталог не возвращается.</span><span class="sxs-lookup"><span data-stu-id="04ab5-110">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="04ab5-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04ab5-111">Permissions</span></span>
<span data-ttu-id="04ab5-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ab5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ab5-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04ab5-114">Permission type</span></span>      | <span data-ttu-id="04ab5-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04ab5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ab5-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04ab5-116">Delegated (work or school account)</span></span> | <span data-ttu-id="04ab5-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04ab5-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04ab5-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04ab5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ab5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04ab5-119">Not supported.</span></span>    |
|<span data-ttu-id="04ab5-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04ab5-120">Application</span></span> | <span data-ttu-id="04ab5-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ab5-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04ab5-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04ab5-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="04ab5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04ab5-123">Request headers</span></span>
| <span data-ttu-id="04ab5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="04ab5-124">Name</span></span>       | <span data-ttu-id="04ab5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="04ab5-125">Type</span></span> | <span data-ttu-id="04ab5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="04ab5-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04ab5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="04ab5-127">Authorization</span></span>  | <span data-ttu-id="04ab5-128">строка</span><span class="sxs-lookup"><span data-stu-id="04ab5-128">string</span></span>  | <span data-ttu-id="04ab5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04ab5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04ab5-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04ab5-131">Request body</span></span>
<span data-ttu-id="04ab5-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="04ab5-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04ab5-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="04ab5-133">Parameter</span></span>    | <span data-ttu-id="04ab5-134">Тип</span><span class="sxs-lookup"><span data-stu-id="04ab5-134">Type</span></span>   |<span data-ttu-id="04ab5-135">Описание</span><span class="sxs-lookup"><span data-stu-id="04ab5-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04ab5-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="04ab5-136">securityEnabledOnly</span></span>|<span data-ttu-id="04ab5-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="04ab5-137">Boolean</span></span>|<span data-ttu-id="04ab5-p106">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="04ab5-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="04ab5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ab5-140">Response</span></span>
<span data-ttu-id="04ab5-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="04ab5-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="04ab5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="04ab5-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="04ab5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="04ab5-143">Request</span></span>
<span data-ttu-id="04ab5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04ab5-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="04ab5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ab5-145">Response</span></span>
<span data-ttu-id="04ab5-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04ab5-146">The following is an example of the response.</span></span>
><span data-ttu-id="04ab5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04ab5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
