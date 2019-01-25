---
title: 'groupLifecyclePolicy: removeGroup'
description: Удаляет группу из политики жизненного цикла.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: b3fd7f46c9c35777468a8436433d034ff000ea5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524886"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="dbf5c-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="dbf5c-103">groupLifecyclePolicy: removeGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbf5c-104">Удаляет группу из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-104">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbf5c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbf5c-105">Permissions</span></span>

<span data-ttu-id="dbf5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbf5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dbf5c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbf5c-108">Permission type</span></span>      | <span data-ttu-id="dbf5c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbf5c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbf5c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbf5c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dbf5c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf5c-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbf5c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbf5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbf5c-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dbf5c-113">Not supported</span></span> |
|<span data-ttu-id="dbf5c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbf5c-114">Application</span></span> |  <span data-ttu-id="dbf5c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf5c-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbf5c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbf5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="dbf5c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbf5c-117">Request headers</span></span>

| <span data-ttu-id="dbf5c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dbf5c-118">Name</span></span> | <span data-ttu-id="dbf5c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf5c-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="dbf5c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbf5c-120">Authorization</span></span> | <span data-ttu-id="dbf5c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbf5c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbf5c-123">Content-Type</span></span>  | <span data-ttu-id="dbf5c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dbf5c-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbf5c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbf5c-125">Request body</span></span>
<span data-ttu-id="dbf5c-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbf5c-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="dbf5c-127">Parameter</span></span> | <span data-ttu-id="dbf5c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dbf5c-128">Type</span></span> | <span data-ttu-id="dbf5c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf5c-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dbf5c-130">groupId</span><span class="sxs-lookup"><span data-stu-id="dbf5c-130">groupId</span></span>|<span data-ttu-id="dbf5c-131">GUID</span><span class="sxs-lookup"><span data-stu-id="dbf5c-131">Guid</span></span>| <span data-ttu-id="dbf5c-132">Идентификатор группы, которую нужно удалить из политики.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-132">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="dbf5c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbf5c-133">Response</span></span>

<span data-ttu-id="dbf5c-134">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="dbf5c-135">Если из политики удаляется группа, в теле отклика возвращается значение **true**.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-135">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="dbf5c-136">Если нет, то в теле отклика возвращается значение **false**.</span><span class="sxs-lookup"><span data-stu-id="dbf5c-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="dbf5c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="dbf5c-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dbf5c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbf5c-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="dbf5c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbf5c-139">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-removegroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
