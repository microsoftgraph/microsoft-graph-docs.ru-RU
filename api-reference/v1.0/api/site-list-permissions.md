---
title: Разрешения списка
description: Получите ресурсы разрешений из свойства навигации разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 86ffad18cc70742a8bc60d7b3475f0af37f49db0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162126"
---
# <a name="list-permissions"></a><span data-ttu-id="0e211-103">Разрешения списка</span><span class="sxs-lookup"><span data-stu-id="0e211-103">List permissions</span></span>
<span data-ttu-id="0e211-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e211-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e211-105">Получите ресурсы [разрешений](../resources/permission.md) из свойства навигации разрешений на сайте.</span><span class="sxs-lookup"><span data-stu-id="0e211-105">Get the [permission](../resources/permission.md) resources from the permissions navigation property on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e211-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e211-106">Permissions</span></span>
<span data-ttu-id="0e211-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e211-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e211-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e211-109">Permission type</span></span>                        | <span data-ttu-id="0e211-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e211-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="0e211-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e211-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e211-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e211-112">Not supported.</span></span>
|<span data-ttu-id="0e211-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e211-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e211-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e211-114">Not supported.</span></span>
|<span data-ttu-id="0e211-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e211-115">Application</span></span>                            | <span data-ttu-id="0e211-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0e211-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0e211-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e211-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e211-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e211-118">Optional query parameters</span></span>
<span data-ttu-id="0e211-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0e211-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0e211-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0e211-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e211-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e211-121">Request headers</span></span>
|<span data-ttu-id="0e211-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0e211-122">Name</span></span>|<span data-ttu-id="0e211-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0e211-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e211-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e211-124">Authorization</span></span>|<span data-ttu-id="0e211-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e211-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e211-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e211-127">Request body</span></span>
<span data-ttu-id="0e211-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e211-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e211-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e211-129">Response</span></span>

<span data-ttu-id="0e211-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [разрешений](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e211-130">If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e211-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e211-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e211-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e211-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_permission"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions
```


### <a name="response"></a><span data-ttu-id="0e211-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e211-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["read"],
      "grantedToIdentities": [{
        "application": {
          "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
          "displayName": "Foo App"
        }
      }]
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedToIdentities": [{
        "application": {
          "id": "22f09bb7-dd29-403e-bec2-ab5cde52c2b3",
          "displayName": "Bar App"
        }
      }]
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/List site permission",
} -->
