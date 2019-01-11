---
title: Назначение руководителя
description: С помощью этого API можно назначить руководителя пользователю.
localization_priority: Normal
ms.openlocfilehash: ddbb73b5306188f2126f7817ddde6d02bde6f850
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877499"
---
# <a name="assign-a-manager"></a><span data-ttu-id="1f651-103">Назначение руководителя</span><span class="sxs-lookup"><span data-stu-id="1f651-103">Assign a manager</span></span>

<span data-ttu-id="1f651-104">С помощью этого API можно назначить руководителя пользователю.</span><span class="sxs-lookup"><span data-stu-id="1f651-104">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="1f651-105">Примечание. Назначать подчиненных невозможно. Вместо этого используйте данный API.</span><span class="sxs-lookup"><span data-stu-id="1f651-105">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f651-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f651-106">Permissions</span></span>
<span data-ttu-id="1f651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f651-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f651-109">Permission type</span></span>      | <span data-ttu-id="1f651-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f651-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f651-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f651-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f651-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f651-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f651-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f651-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f651-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f651-114">Not supported.</span></span>    |
|<span data-ttu-id="1f651-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f651-115">Application</span></span> | <span data-ttu-id="1f651-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f651-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f651-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f651-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1f651-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f651-118">Request headers</span></span>
| <span data-ttu-id="1f651-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1f651-119">Name</span></span>       | <span data-ttu-id="1f651-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1f651-120">Type</span></span> | <span data-ttu-id="1f651-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1f651-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f651-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f651-122">Authorization</span></span>  | <span data-ttu-id="1f651-123">string</span><span class="sxs-lookup"><span data-stu-id="1f651-123">string</span></span>  | <span data-ttu-id="1f651-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f651-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f651-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f651-126">Request body</span></span>
<span data-ttu-id="1f651-127">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f651-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="1f651-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f651-128">Response</span></span>

<span data-ttu-id="1f651-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1f651-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f651-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1f651-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f651-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f651-132">Request</span></span>
<span data-ttu-id="1f651-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f651-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="1f651-134">Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f651-134">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="1f651-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f651-135">Response</span></span>
<span data-ttu-id="1f651-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1f651-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
