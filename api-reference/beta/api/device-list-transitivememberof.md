---
title: Доверия транзитивных групп списка устройств
description: Получите, устройство является членом группы. Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e894a423675acb498af555f003e75fd9d412091
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353085"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="22b4e-104">Доверия транзитивных групп списка устройств</span><span class="sxs-lookup"><span data-stu-id="22b4e-104">List device transitive groups</span></span>

> <span data-ttu-id="22b4e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22b4e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22b4e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22b4e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22b4e-107">Получите, устройство является членом группы.</span><span class="sxs-lookup"><span data-stu-id="22b4e-107">Get groups that the device is a member of.</span></span> <span data-ttu-id="22b4e-108">Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.</span><span class="sxs-lookup"><span data-stu-id="22b4e-108">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="22b4e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22b4e-109">Permissions</span></span>

<span data-ttu-id="22b4e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22b4e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22b4e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22b4e-112">Permission type</span></span>      | <span data-ttu-id="22b4e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22b4e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22b4e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22b4e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="22b4e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22b4e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22b4e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22b4e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22b4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22b4e-117">Not supported.</span></span>    |
|<span data-ttu-id="22b4e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22b4e-118">Application</span></span> | <span data-ttu-id="22b4e-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22b4e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22b4e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22b4e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22b4e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="22b4e-121">Optional query parameters</span></span>

<span data-ttu-id="22b4e-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="22b4e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22b4e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22b4e-123">Request headers</span></span>

| <span data-ttu-id="22b4e-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22b4e-124">Header</span></span>       | <span data-ttu-id="22b4e-125">Значение</span><span class="sxs-lookup"><span data-stu-id="22b4e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22b4e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22b4e-126">Authorization</span></span>  | <span data-ttu-id="22b4e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22b4e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="22b4e-129">Accept</span><span class="sxs-lookup"><span data-stu-id="22b4e-129">Accept</span></span>  | <span data-ttu-id="22b4e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="22b4e-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22b4e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22b4e-131">Request body</span></span>

<span data-ttu-id="22b4e-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22b4e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22b4e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="22b4e-133">Response</span></span>

<span data-ttu-id="22b4e-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22b4e-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22b4e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="22b4e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="22b4e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="22b4e-136">Request</span></span>

<span data-ttu-id="22b4e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22b4e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="22b4e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="22b4e-138">Response</span></span>

<span data-ttu-id="22b4e-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="22b4e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
