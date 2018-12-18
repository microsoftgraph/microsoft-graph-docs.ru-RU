---
title: Список scopedMembers для роли каталога
description: Получение списка объектов scopedRoleMembership для роли каталога.
author: lleonard-msft
ms.openlocfilehash: b3d0e8bc67b6ab670b7dc8a149bad0f031b03762
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311720"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="d86fc-103">Список scopedMembers для роли каталога</span><span class="sxs-lookup"><span data-stu-id="d86fc-103">List scopedMembers for a directory role</span></span>

> <span data-ttu-id="d86fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d86fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d86fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d86fc-106">Получение списка объектов [scopedRoleMembership](../resources/scopedrolemembership.md) для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="d86fc-106">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="d86fc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d86fc-107">Permissions</span></span>
<span data-ttu-id="d86fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d86fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d86fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d86fc-110">Permission type</span></span>      | <span data-ttu-id="d86fc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d86fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d86fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d86fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d86fc-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d86fc-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d86fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d86fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d86fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86fc-115">Not supported.</span></span>    |
|<span data-ttu-id="d86fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d86fc-116">Application</span></span> | <span data-ttu-id="d86fc-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86fc-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d86fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d86fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d86fc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d86fc-119">Optional query parameters</span></span>
<span data-ttu-id="d86fc-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d86fc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d86fc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d86fc-121">Request headers</span></span>
| <span data-ttu-id="d86fc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d86fc-122">Name</span></span>      |<span data-ttu-id="d86fc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d86fc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d86fc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d86fc-124">Authorization</span></span>  | <span data-ttu-id="d86fc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d86fc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d86fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d86fc-127">Request body</span></span>
<span data-ttu-id="d86fc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d86fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d86fc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d86fc-129">Response</span></span>

<span data-ttu-id="d86fc-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [scopedRoleMembership](../resources/scopedrolemembership.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d86fc-130">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d86fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d86fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d86fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d86fc-132">Request</span></span>
<span data-ttu-id="d86fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d86fc-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
##### <a name="response"></a><span data-ttu-id="d86fc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d86fc-134">Response</span></span>
<span data-ttu-id="d86fc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d86fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->