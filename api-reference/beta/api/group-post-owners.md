---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 049c860be95e2f4f4b83848d8d8be6b3dd0ed9c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517171"
---
# <a name="add-group-owner"></a><span data-ttu-id="fc20c-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="fc20c-104">Add group owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc20c-p102">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="fc20c-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="fc20c-107">**Важные:** При изменении группы владельцев и созданных групп для группы, может потребоваться до 2 часа для владельцев для синхронизации с группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fc20c-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="fc20c-108">Кроме того Если владелец могут вносить изменения в группе — например, путем создания плана планировщик работы - владелец также необходимо добавить как участник группы/группы.</span><span class="sxs-lookup"><span data-stu-id="fc20c-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fc20c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc20c-109">Permissions</span></span>
<span data-ttu-id="fc20c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc20c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc20c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc20c-112">Permission type</span></span>      | <span data-ttu-id="fc20c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc20c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc20c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc20c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fc20c-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc20c-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc20c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc20c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc20c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc20c-117">Not supported.</span></span>    |
|<span data-ttu-id="fc20c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc20c-118">Application</span></span> | <span data-ttu-id="fc20c-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc20c-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc20c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc20c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fc20c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc20c-121">Request headers</span></span>
| <span data-ttu-id="fc20c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fc20c-122">Name</span></span>       | <span data-ttu-id="fc20c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fc20c-123">Type</span></span> | <span data-ttu-id="fc20c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fc20c-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc20c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc20c-125">Authorization</span></span>  | <span data-ttu-id="fc20c-126">string</span><span class="sxs-lookup"><span data-stu-id="fc20c-126">string</span></span>  | <span data-ttu-id="fc20c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc20c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc20c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc20c-129">Request body</span></span>
<span data-ttu-id="fc20c-130">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc20c-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="fc20c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc20c-131">Response</span></span>
<span data-ttu-id="fc20c-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fc20c-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc20c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fc20c-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fc20c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc20c-135">Request</span></span>
<span data-ttu-id="fc20c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc20c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
<span data-ttu-id="fc20c-137">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc20c-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="fc20c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc20c-138">Response</span></span>
<span data-ttu-id="fc20c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc20c-139">The following is an example of the response.</span></span>
><span data-ttu-id="fc20c-140">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc20c-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fc20c-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc20c-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
