---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
ms.openlocfilehash: 903c659722877263038860c7d2ff47b301b6d5c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308899"
---
# <a name="add-group-owner"></a><span data-ttu-id="79217-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="79217-104">Add group owner</span></span>

> <span data-ttu-id="79217-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79217-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79217-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79217-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79217-p103">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="79217-p103">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="79217-109">**Важные:** При изменении группы владельцев и созданных групп для группы, может потребоваться до 2 часа для владельцев для синхронизации с группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="79217-109">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="79217-110">Кроме того Если владелец могут вносить изменения в группе — например, путем создания плана планировщик работы - владелец также необходимо добавить как участник группы/группы.</span><span class="sxs-lookup"><span data-stu-id="79217-110">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="79217-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79217-111">Permissions</span></span>
<span data-ttu-id="79217-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79217-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79217-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79217-114">Permission type</span></span>      | <span data-ttu-id="79217-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79217-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79217-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79217-116">Delegated (work or school account)</span></span> | <span data-ttu-id="79217-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79217-117">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="79217-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79217-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79217-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79217-119">Not supported.</span></span>    |
|<span data-ttu-id="79217-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79217-120">Application</span></span> | <span data-ttu-id="79217-121">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79217-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79217-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79217-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="79217-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79217-123">Request headers</span></span>
| <span data-ttu-id="79217-124">Имя</span><span class="sxs-lookup"><span data-stu-id="79217-124">Name</span></span>       | <span data-ttu-id="79217-125">Тип</span><span class="sxs-lookup"><span data-stu-id="79217-125">Type</span></span> | <span data-ttu-id="79217-126">Описание</span><span class="sxs-lookup"><span data-stu-id="79217-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79217-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="79217-127">Authorization</span></span>  | <span data-ttu-id="79217-128">string</span><span class="sxs-lookup"><span data-stu-id="79217-128">string</span></span>  | <span data-ttu-id="79217-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79217-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79217-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79217-131">Request body</span></span>
<span data-ttu-id="79217-132">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79217-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="79217-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="79217-133">Response</span></span>
<span data-ttu-id="79217-p107">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="79217-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79217-136">Пример</span><span class="sxs-lookup"><span data-stu-id="79217-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="79217-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="79217-137">Request</span></span>
<span data-ttu-id="79217-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79217-138">The following is an example of the request.</span></span>
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
<span data-ttu-id="79217-139">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79217-139">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="79217-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="79217-140">Response</span></span>
<span data-ttu-id="79217-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79217-141">The following is an example of the response.</span></span>
><span data-ttu-id="79217-142">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="79217-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79217-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79217-143">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
