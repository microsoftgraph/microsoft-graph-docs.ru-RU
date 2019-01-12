---
title: Назначение руководителя
description: С помощью этого API можно назначить руководителя пользователю.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 770fad522e505abbd9f689540e6a28e875ba063d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912073"
---
# <a name="assign-a-manager"></a><span data-ttu-id="aa7d9-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="aa7d9-103">Assign a manager</span></span>

> <span data-ttu-id="aa7d9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa7d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa7d9-106">С помощью этого API можно назначить руководителя пользователю.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-106">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="aa7d9-107">Примечание. Назначать подчиненных невозможно. Вместо этого используйте данный API.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-107">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa7d9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa7d9-108">Permissions</span></span>
<span data-ttu-id="aa7d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa7d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa7d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa7d9-111">Permission type</span></span>      | <span data-ttu-id="aa7d9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa7d9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa7d9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa7d9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aa7d9-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa7d9-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa7d9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa7d9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa7d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-116">Not supported.</span></span>    |
|<span data-ttu-id="aa7d9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa7d9-117">Application</span></span> | <span data-ttu-id="aa7d9-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa7d9-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa7d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa7d9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="aa7d9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa7d9-120">Request headers</span></span>
| <span data-ttu-id="aa7d9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="aa7d9-121">Name</span></span>       | <span data-ttu-id="aa7d9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="aa7d9-122">Type</span></span> | <span data-ttu-id="aa7d9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aa7d9-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa7d9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa7d9-124">Authorization</span></span>  | <span data-ttu-id="aa7d9-125">string</span><span class="sxs-lookup"><span data-stu-id="aa7d9-125">string</span></span>  | <span data-ttu-id="aa7d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa7d9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa7d9-128">Request body</span></span>
<span data-ttu-id="aa7d9-129">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-129">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="aa7d9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa7d9-130">Response</span></span>

<span data-ttu-id="aa7d9-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa7d9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aa7d9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa7d9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa7d9-134">Request</span></span>
<span data-ttu-id="aa7d9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="aa7d9-136">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-136">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="aa7d9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa7d9-137">Response</span></span>
<span data-ttu-id="aa7d9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aa7d9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
