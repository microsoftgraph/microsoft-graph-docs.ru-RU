---
title: Добавление участника
description: С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
ms.openlocfilehash: 1fe2d5c259b4e1974168df30e282d97d3342e0bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026352"
---
# <a name="add-member"></a><span data-ttu-id="6ab26-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="6ab26-103">Add member</span></span>
<span data-ttu-id="6ab26-104">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="6ab26-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="6ab26-105">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="6ab26-105">You can add users or other groups.</span></span> <span data-ttu-id="6ab26-106">Важно! В Группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="6ab26-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ab26-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ab26-107">Permissions</span></span>
<span data-ttu-id="6ab26-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ab26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab26-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ab26-110">Permission type</span></span>      | <span data-ttu-id="6ab26-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ab26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ab26-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ab26-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ab26-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ab26-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ab26-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ab26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ab26-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ab26-115">Not supported.</span></span>    |
|<span data-ttu-id="6ab26-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6ab26-116">Application</span></span> | <span data-ttu-id="6ab26-117">Group.ReadWrite.All и Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab26-117">Group.ReadWrite.All and Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ab26-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ab26-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6ab26-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ab26-119">Request headers</span></span>
| <span data-ttu-id="6ab26-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ab26-120">Name</span></span>       | <span data-ttu-id="6ab26-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6ab26-121">Type</span></span> | <span data-ttu-id="6ab26-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab26-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ab26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ab26-123">Authorization</span></span>  | <span data-ttu-id="6ab26-124">string</span><span class="sxs-lookup"><span data-stu-id="6ab26-124">string</span></span>  | <span data-ttu-id="6ab26-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ab26-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ab26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ab26-127">Request body</span></span>
<span data-ttu-id="6ab26-128">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ab26-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="6ab26-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ab26-129">Response</span></span>
<span data-ttu-id="6ab26-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6ab26-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ab26-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6ab26-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6ab26-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ab26-133">Request</span></span>
<span data-ttu-id="6ab26-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ab26-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="6ab26-135">Укажите в тексте запроса свойство `id` добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md), представленное в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ab26-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="6ab26-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ab26-136">Response</span></span>
<span data-ttu-id="6ab26-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6ab26-137">The following is an example of the response.</span></span>
><span data-ttu-id="6ab26-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="6ab26-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6ab26-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ab26-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->