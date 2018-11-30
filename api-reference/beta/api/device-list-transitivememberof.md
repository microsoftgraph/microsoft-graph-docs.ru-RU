---
title: Доверия транзитивных групп списка устройств
description: Получите, устройство является членом группы. Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.
ms.openlocfilehash: 39589ec7c1858d773ed0907950142ec3b1f4cdef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075267"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="bd9ab-104">Доверия транзитивных групп списка устройств</span><span class="sxs-lookup"><span data-stu-id="bd9ab-104">List device transitive groups</span></span>

> <span data-ttu-id="bd9ab-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd9ab-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd9ab-107">Получите, устройство является членом группы.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-107">Get groups that the device is a member of.</span></span> <span data-ttu-id="bd9ab-108">Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-108">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd9ab-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd9ab-109">Permissions</span></span>

<span data-ttu-id="bd9ab-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9ab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd9ab-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd9ab-112">Permission type</span></span>      | <span data-ttu-id="bd9ab-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd9ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd9ab-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd9ab-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bd9ab-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd9ab-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bd9ab-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd9ab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd9ab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-117">Not supported.</span></span>    |
|<span data-ttu-id="bd9ab-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd9ab-118">Application</span></span> | <span data-ttu-id="bd9ab-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9ab-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd9ab-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd9ab-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd9ab-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd9ab-121">Optional query parameters</span></span>

<span data-ttu-id="bd9ab-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd9ab-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd9ab-123">Request headers</span></span>

| <span data-ttu-id="bd9ab-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd9ab-124">Header</span></span>       | <span data-ttu-id="bd9ab-125">Значение</span><span class="sxs-lookup"><span data-stu-id="bd9ab-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd9ab-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd9ab-126">Authorization</span></span>  | <span data-ttu-id="bd9ab-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd9ab-129">Accept</span><span class="sxs-lookup"><span data-stu-id="bd9ab-129">Accept</span></span>  | <span data-ttu-id="bd9ab-130">application/json</span><span class="sxs-lookup"><span data-stu-id="bd9ab-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd9ab-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd9ab-131">Request body</span></span>

<span data-ttu-id="bd9ab-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd9ab-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd9ab-133">Response</span></span>

<span data-ttu-id="bd9ab-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd9ab-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bd9ab-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd9ab-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd9ab-136">Request</span></span>

<span data-ttu-id="bd9ab-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd9ab-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="bd9ab-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd9ab-138">Response</span></span>

<span data-ttu-id="bd9ab-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bd9ab-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->