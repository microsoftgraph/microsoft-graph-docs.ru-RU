---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b9020c4fad74990a18023bdddd63ae3bd050998
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455277"
---
# <a name="list-registeredowners"></a><span data-ttu-id="de613-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="de613-106">List registeredOwners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de613-107">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="de613-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="de613-108">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="de613-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="de613-109">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="de613-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="de613-110">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="de613-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="de613-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de613-111">Permissions</span></span>

<span data-ttu-id="de613-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de613-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de613-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de613-114">Permission type</span></span>      | <span data-ttu-id="de613-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de613-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de613-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de613-116">Delegated (work or school account)</span></span> | <span data-ttu-id="de613-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de613-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de613-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de613-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de613-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de613-119">Not supported.</span></span>    |
|<span data-ttu-id="de613-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de613-120">Application</span></span> | <span data-ttu-id="de613-121">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de613-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de613-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de613-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="de613-123">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="de613-123">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="de613-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="de613-124">Optional query parameters</span></span>
<span data-ttu-id="de613-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="de613-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="de613-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de613-126">Request headers</span></span>
| <span data-ttu-id="de613-127">Имя</span><span class="sxs-lookup"><span data-stu-id="de613-127">Name</span></span>       | <span data-ttu-id="de613-128">Тип</span><span class="sxs-lookup"><span data-stu-id="de613-128">Type</span></span> | <span data-ttu-id="de613-129">Описание</span><span class="sxs-lookup"><span data-stu-id="de613-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de613-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="de613-130">Authorization</span></span>  | <span data-ttu-id="de613-131">string</span><span class="sxs-lookup"><span data-stu-id="de613-131">string</span></span>  | <span data-ttu-id="de613-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de613-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de613-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de613-134">Request body</span></span>
<span data-ttu-id="de613-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de613-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de613-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="de613-136">Response</span></span>

<span data-ttu-id="de613-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de613-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de613-138">Пример</span><span class="sxs-lookup"><span data-stu-id="de613-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de613-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="de613-139">Request</span></span>
<span data-ttu-id="de613-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de613-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="de613-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="de613-141">Response</span></span>
<span data-ttu-id="de613-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de613-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-registeredowners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
