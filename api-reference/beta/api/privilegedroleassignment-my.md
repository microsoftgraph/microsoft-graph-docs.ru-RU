---
title: 'privilegedRoleAssignment: Мой'
description: Получение назначения ролей привилегированной инициатора.
ms.openlocfilehash: 7291d7ae27804c633f98a24ed7c36170e77c61e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077603"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="9d663-103">privilegedRoleAssignment: Мой</span><span class="sxs-lookup"><span data-stu-id="9d663-103">privilegedRoleAssignment: my</span></span>

> <span data-ttu-id="9d663-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d663-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d663-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d663-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d663-106">Получение назначения ролей привилегированной инициатора.</span><span class="sxs-lookup"><span data-stu-id="9d663-106">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d663-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d663-107">Permissions</span></span>
<span data-ttu-id="9d663-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d663-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d663-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d663-110">Permission type</span></span>      | <span data-ttu-id="9d663-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d663-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d663-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d663-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d663-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d663-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d663-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d663-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d663-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d663-115">Not supported.</span></span>    |
|<span data-ttu-id="9d663-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d663-116">Application</span></span> | <span data-ttu-id="9d663-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d663-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d663-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d663-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="9d663-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d663-119">Request headers</span></span>
| <span data-ttu-id="9d663-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9d663-120">Name</span></span>       | <span data-ttu-id="9d663-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9d663-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d663-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d663-122">Authorization</span></span>  | <span data-ttu-id="9d663-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d663-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d663-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d663-125">Request body</span></span>
<span data-ttu-id="9d663-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d663-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d663-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d663-127">Response</span></span>

<span data-ttu-id="9d663-128">Успешно завершена, этот метод возвращает `200 OK` кода и [privilegedRoleAssignment](../resources/privilegedroleassignment.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9d663-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d663-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9d663-129">Example</span></span>
<span data-ttu-id="9d663-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9d663-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9d663-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d663-131">Request</span></span>
<span data-ttu-id="9d663-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d663-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="9d663-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d663-133">Response</span></span>
<span data-ttu-id="9d663-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9d663-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->