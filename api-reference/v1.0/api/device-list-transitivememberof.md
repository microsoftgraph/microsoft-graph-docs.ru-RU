---
title: Доверия транзитивных групп списка устройств
description: Получите, устройство является членом группы. Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: fbe7aee8066c56ad9f49dd2ad77fedfe0b75fbfc
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694498"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="4eae0-104">Доверия транзитивных групп списка устройств</span><span class="sxs-lookup"><span data-stu-id="4eae0-104">List device transitive groups</span></span>

<span data-ttu-id="4eae0-105">Получите, устройство является членом группы.</span><span class="sxs-lookup"><span data-stu-id="4eae0-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="4eae0-106">Этот запрос API доверия транзитивных и также возвращает все группы, устройство является участником вложенных.</span><span class="sxs-lookup"><span data-stu-id="4eae0-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4eae0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4eae0-107">Permissions</span></span>

<span data-ttu-id="4eae0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eae0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eae0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eae0-110">Permission type</span></span>      | <span data-ttu-id="4eae0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eae0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4eae0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eae0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4eae0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4eae0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4eae0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eae0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eae0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eae0-115">Not supported.</span></span>    |
|<span data-ttu-id="4eae0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eae0-116">Application</span></span> | <span data-ttu-id="4eae0-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eae0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eae0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eae0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4eae0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4eae0-119">Optional query parameters</span></span>

<span data-ttu-id="4eae0-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4eae0-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eae0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eae0-121">Request headers</span></span>

| <span data-ttu-id="4eae0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eae0-122">Header</span></span>       | <span data-ttu-id="4eae0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4eae0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4eae0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4eae0-124">Authorization</span></span>  | <span data-ttu-id="4eae0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eae0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4eae0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4eae0-127">Accept</span></span>  | <span data-ttu-id="4eae0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4eae0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eae0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eae0-129">Request body</span></span>

<span data-ttu-id="4eae0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eae0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eae0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eae0-131">Response</span></span>

<span data-ttu-id="4eae0-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eae0-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eae0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4eae0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eae0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eae0-134">Request</span></span>

<span data-ttu-id="4eae0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eae0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="4eae0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4eae0-136">Response</span></span>

<span data-ttu-id="4eae0-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4eae0-137">Here is an example of the response.</span></span> 

><span data-ttu-id="4eae0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eae0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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