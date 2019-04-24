---
title: Добавление участника
description: С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ac21262858137074ed92978f0ab6530052fcc2de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502189"
---
# <a name="add-member"></a><span data-ttu-id="dfeef-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="dfeef-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfeef-104">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="dfeef-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="dfeef-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="dfeef-105">You can add users or other groups.</span></span> <span data-ttu-id="dfeef-106">Важно! В Группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="dfeef-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfeef-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfeef-107">Permissions</span></span>
<span data-ttu-id="dfeef-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfeef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfeef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfeef-110">Permission type</span></span>      | <span data-ttu-id="dfeef-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfeef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfeef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfeef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dfeef-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfeef-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfeef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfeef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfeef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfeef-115">Not supported.</span></span>    |
|<span data-ttu-id="dfeef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfeef-116">Application</span></span> | <span data-ttu-id="dfeef-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfeef-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfeef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfeef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="dfeef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfeef-119">Request headers</span></span>
| <span data-ttu-id="dfeef-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dfeef-120">Name</span></span>       | <span data-ttu-id="dfeef-121">Тип</span><span class="sxs-lookup"><span data-stu-id="dfeef-121">Type</span></span> | <span data-ttu-id="dfeef-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dfeef-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfeef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfeef-123">Authorization</span></span>  | <span data-ttu-id="dfeef-124">string</span><span class="sxs-lookup"><span data-stu-id="dfeef-124">string</span></span>  | <span data-ttu-id="dfeef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfeef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfeef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfeef-127">Request body</span></span>
<span data-ttu-id="dfeef-128">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfeef-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="dfeef-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfeef-129">Response</span></span>
<span data-ttu-id="dfeef-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dfeef-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfeef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dfeef-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dfeef-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfeef-133">Request</span></span>
<span data-ttu-id="dfeef-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfeef-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="dfeef-135">В тексте запроса добавьте `id` представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [группы](../resources/group.md) , который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfeef-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="dfeef-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfeef-136">Response</span></span>
<span data-ttu-id="dfeef-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfeef-137">The following is an example of the response.</span></span>
><span data-ttu-id="dfeef-138">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dfeef-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dfeef-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfeef-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
