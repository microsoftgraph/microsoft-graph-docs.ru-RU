---
title: Список Екстерналспонсорс
description: Получение списка Екстерналспонсорс Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a523c0a75b6cffb20738f42f33554accbe945c18
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757481"
---
# <a name="list-externalsponsors"></a><span data-ttu-id="de479-103">Список Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="de479-103">List externalSponsors</span></span>

<span data-ttu-id="de479-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de479-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de479-105">Получение списка внешних спонсоров [коннектедорганизатион](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="de479-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s external sponsors.</span></span>  <span data-ttu-id="de479-106">Внешние спонсоры — это набор пользователей, которые могут утверждать запросы от имени других пользователей из этой подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="de479-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="de479-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de479-107">Permissions</span></span>

<span data-ttu-id="de479-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de479-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de479-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de479-110">Permission type</span></span>|<span data-ttu-id="de479-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de479-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="de479-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de479-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="de479-113">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de479-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="de479-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de479-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de479-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de479-115">Not supported.</span></span> |
| <span data-ttu-id="de479-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de479-116">Application</span></span>                            | <span data-ttu-id="de479-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de479-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de479-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de479-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="de479-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de479-119">Request headers</span></span>
|<span data-ttu-id="de479-120">Имя</span><span class="sxs-lookup"><span data-stu-id="de479-120">Name</span></span>|<span data-ttu-id="de479-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de479-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de479-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de479-122">Authorization</span></span>|<span data-ttu-id="de479-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de479-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de479-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de479-125">Request body</span></span>
<span data-ttu-id="de479-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de479-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de479-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="de479-127">Response</span></span>

<span data-ttu-id="de479-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de479-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de479-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="de479-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de479-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="de479-130">Request</span></span>

<span data-ttu-id="de479-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de479-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_externalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

### <a name="response"></a><span data-ttu-id="de479-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="de479-132">Response</span></span>

<span data-ttu-id="de479-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de479-133">The following is an example of the response.</span></span>

<span data-ttu-id="de479-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de479-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List externalSponsors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
