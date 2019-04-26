---
title: Назначение руководителя
description: С помощью этого API можно назначить руководителя пользователю.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 777e086a99af68e39b093115502809784e604ec2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329804"
---
# <a name="assign-a-manager"></a><span data-ttu-id="93d0a-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="93d0a-103">Assign a manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93d0a-104">С помощью этого API можно назначить руководителя пользователю.</span><span class="sxs-lookup"><span data-stu-id="93d0a-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="93d0a-105">Примечание. Назначать подчиненных невозможно. Вместо этого используйте данный API.</span><span class="sxs-lookup"><span data-stu-id="93d0a-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93d0a-106">Permissions</span></span>
<span data-ttu-id="93d0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93d0a-109">Permission type</span></span>      | <span data-ttu-id="93d0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93d0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93d0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93d0a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93d0a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93d0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93d0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93d0a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93d0a-114">Not supported.</span></span>    |
|<span data-ttu-id="93d0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93d0a-115">Application</span></span> | <span data-ttu-id="93d0a-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d0a-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93d0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93d0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="93d0a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93d0a-118">Request headers</span></span>
| <span data-ttu-id="93d0a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="93d0a-119">Name</span></span>       | <span data-ttu-id="93d0a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="93d0a-120">Type</span></span> | <span data-ttu-id="93d0a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="93d0a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="93d0a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93d0a-122">Authorization</span></span>  | <span data-ttu-id="93d0a-123">string</span><span class="sxs-lookup"><span data-stu-id="93d0a-123">string</span></span>  | <span data-ttu-id="93d0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93d0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93d0a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93d0a-126">Request body</span></span>
<span data-ttu-id="93d0a-127">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93d0a-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="93d0a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d0a-128">Response</span></span>

<span data-ttu-id="93d0a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="93d0a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93d0a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="93d0a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93d0a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d0a-132">Request</span></span>
<span data-ttu-id="93d0a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d0a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="93d0a-134">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93d0a-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="93d0a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d0a-135">Response</span></span>
<span data-ttu-id="93d0a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93d0a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
