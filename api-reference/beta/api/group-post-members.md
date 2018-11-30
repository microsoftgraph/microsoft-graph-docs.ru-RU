---
title: Добавление участника
description: С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.
ms.openlocfilehash: 3ebfad3b3e1fe2c3411653108d75d44d0fc53913
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074597"
---
# <a name="add-member"></a><span data-ttu-id="61fa1-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="61fa1-103">Add member</span></span>

> <span data-ttu-id="61fa1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="61fa1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61fa1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61fa1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61fa1-106">С помощью этого API можно добавить участника в группу Office 365 или группу безопасности (обычную или с поддержкой почты) через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="61fa1-106">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="61fa1-107">Вы можете добавлять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="61fa1-107">You can add users or other groups.</span></span> <span data-ttu-id="61fa1-108">Важно! В Группы Office 365 можно добавлять только пользователей.</span><span class="sxs-lookup"><span data-stu-id="61fa1-108">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="61fa1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61fa1-109">Permissions</span></span>
<span data-ttu-id="61fa1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61fa1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61fa1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61fa1-112">Permission type</span></span>      | <span data-ttu-id="61fa1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61fa1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61fa1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61fa1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="61fa1-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61fa1-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61fa1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61fa1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61fa1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61fa1-117">Not supported.</span></span>    |
|<span data-ttu-id="61fa1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61fa1-118">Application</span></span> | <span data-ttu-id="61fa1-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61fa1-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61fa1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61fa1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="61fa1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61fa1-121">Request headers</span></span>
| <span data-ttu-id="61fa1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="61fa1-122">Name</span></span>       | <span data-ttu-id="61fa1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="61fa1-123">Type</span></span> | <span data-ttu-id="61fa1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="61fa1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="61fa1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="61fa1-125">Authorization</span></span>  | <span data-ttu-id="61fa1-126">string</span><span class="sxs-lookup"><span data-stu-id="61fa1-126">string</span></span>  | <span data-ttu-id="61fa1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61fa1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61fa1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61fa1-129">Request body</span></span>
<span data-ttu-id="61fa1-130">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61fa1-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="61fa1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="61fa1-131">Response</span></span>
<span data-ttu-id="61fa1-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="61fa1-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61fa1-134">Пример</span><span class="sxs-lookup"><span data-stu-id="61fa1-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="61fa1-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="61fa1-135">Request</span></span>
<span data-ttu-id="61fa1-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61fa1-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="61fa1-137">В тексте запроса укажите представление JSON `id` объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [группы,](../resources/group.md) необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="61fa1-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="61fa1-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="61fa1-138">Response</span></span>
<span data-ttu-id="61fa1-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="61fa1-139">The following is an example of the response.</span></span>
><span data-ttu-id="61fa1-140">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="61fa1-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="61fa1-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61fa1-141">All the properties will be returned from an actual call.</span></span>
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