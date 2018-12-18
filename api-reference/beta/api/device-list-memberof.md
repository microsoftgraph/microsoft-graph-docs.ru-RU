---
title: Список групп устройств
description: Получите группы, это устройство является непосредственным членом. Эта операция не транзитивное.
author: tfitzmac
ms.openlocfilehash: da0001ab6a609e6f262aa6880306977b9c655b01
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336493"
---
# <a name="list-device-groups"></a><span data-ttu-id="fa305-104">Список групп устройств</span><span class="sxs-lookup"><span data-stu-id="fa305-104">List device groups</span></span>

> <span data-ttu-id="fa305-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa305-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa305-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa305-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa305-107">Получите группы, это устройство является непосредственным членом.</span><span class="sxs-lookup"><span data-stu-id="fa305-107">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="fa305-108">Эта операция не транзитивное.</span><span class="sxs-lookup"><span data-stu-id="fa305-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa305-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa305-109">Permissions</span></span>

<span data-ttu-id="fa305-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa305-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa305-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa305-112">Permission type</span></span>      | <span data-ttu-id="fa305-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa305-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa305-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa305-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fa305-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa305-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa305-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa305-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa305-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa305-117">Not supported.</span></span>    |
|<span data-ttu-id="fa305-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa305-118">Application</span></span> | <span data-ttu-id="fa305-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa305-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa305-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa305-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa305-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa305-121">Optional query parameters</span></span>
<span data-ttu-id="fa305-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa305-122">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fa305-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa305-123">Request headers</span></span>
| <span data-ttu-id="fa305-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa305-124">Header</span></span>       | <span data-ttu-id="fa305-125">Значение</span><span class="sxs-lookup"><span data-stu-id="fa305-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa305-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa305-126">Authorization</span></span>  | <span data-ttu-id="fa305-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa305-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fa305-129">Accept</span><span class="sxs-lookup"><span data-stu-id="fa305-129">Accept</span></span>  | <span data-ttu-id="fa305-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fa305-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa305-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa305-131">Request body</span></span>
<span data-ttu-id="fa305-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa305-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa305-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa305-133">Response</span></span>

<span data-ttu-id="fa305-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa305-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa305-135">Пример</span><span class="sxs-lookup"><span data-stu-id="fa305-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa305-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa305-136">Request</span></span>

<span data-ttu-id="fa305-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa305-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="fa305-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa305-138">Response</span></span>
<span data-ttu-id="fa305-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fa305-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->S