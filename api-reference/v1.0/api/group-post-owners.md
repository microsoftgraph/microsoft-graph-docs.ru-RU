---
title: Добавление владельца группы
description: Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: b3057a270aa2c503d96747e173cc54b13013ce6a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585064"
---
# <a name="add-group-owner"></a><span data-ttu-id="f8f69-104">Добавление владельца группы</span><span class="sxs-lookup"><span data-stu-id="f8f69-104">Add group owner</span></span>
<span data-ttu-id="f8f69-p102">Добавление пользователя в качестве владельца группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="f8f69-p102">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

><span data-ttu-id="f8f69-107">**Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f8f69-107">**Important:** If you update the group owners and you created a team for the group, it can take up to 2 hours for the owners to be synchronized with Microsoft Teams.</span></span> <span data-ttu-id="f8f69-108">Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.</span><span class="sxs-lookup"><span data-stu-id="f8f69-108">Also, if you want the owner to be able to make changes in a team - for example, by creating a Planner plan - the owner also needs to be added as a group/team member.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f8f69-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8f69-109">Permissions</span></span>
<span data-ttu-id="f8f69-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8f69-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8f69-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8f69-112">Permission type</span></span>      | <span data-ttu-id="f8f69-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8f69-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8f69-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8f69-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f8f69-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8f69-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8f69-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8f69-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8f69-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8f69-117">Not supported.</span></span>    |
|<span data-ttu-id="f8f69-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="f8f69-118">Application</span></span> | <span data-ttu-id="f8f69-119">Group.ReadWrite.All и User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f69-119">Group.ReadWrite.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8f69-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8f69-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f8f69-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8f69-121">Request headers</span></span>
| <span data-ttu-id="f8f69-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f8f69-122">Name</span></span>       | <span data-ttu-id="f8f69-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f8f69-123">Type</span></span> | <span data-ttu-id="f8f69-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f8f69-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8f69-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8f69-125">Authorization</span></span>  | <span data-ttu-id="f8f69-126">string</span><span class="sxs-lookup"><span data-stu-id="f8f69-126">string</span></span>  | <span data-ttu-id="f8f69-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8f69-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8f69-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8f69-129">Request body</span></span>
<span data-ttu-id="f8f69-130">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8f69-130">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="f8f69-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8f69-131">Response</span></span>
<span data-ttu-id="f8f69-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f8f69-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f69-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f8f69-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f8f69-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8f69-135">Request</span></span>
<span data-ttu-id="f8f69-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8f69-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="f8f69-137">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8f69-137">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

#### <a name="response"></a><span data-ttu-id="f8f69-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8f69-138">Response</span></span>
<span data-ttu-id="f8f69-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f8f69-139">The following is an example of the response.</span></span>
><span data-ttu-id="f8f69-140">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f8f69-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f8f69-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8f69-141">All the properties will be returned from an actual call.</span></span>
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

