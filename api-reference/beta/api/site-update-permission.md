---
title: Обновление разрешения
description: Обновление объекта разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0bf32370cf83176d79c1766d74036e5afb273297
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160852"
---
# <a name="update-permission"></a><span data-ttu-id="afdf1-103">Обновление разрешения</span><span class="sxs-lookup"><span data-stu-id="afdf1-103">Update permission</span></span>
<span data-ttu-id="afdf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afdf1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afdf1-105">Обновление объекта [разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="afdf1-105">Update the [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="afdf1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afdf1-106">Permissions</span></span>
<span data-ttu-id="afdf1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afdf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afdf1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afdf1-109">Permission type</span></span>                        | <span data-ttu-id="afdf1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afdf1-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="afdf1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afdf1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="afdf1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afdf1-112">Not supported.</span></span>
|<span data-ttu-id="afdf1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afdf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afdf1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afdf1-114">Not supported.</span></span>
|<span data-ttu-id="afdf1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afdf1-115">Application</span></span>                            | <span data-ttu-id="afdf1-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="afdf1-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="afdf1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afdf1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="afdf1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afdf1-118">Request headers</span></span>
|<span data-ttu-id="afdf1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="afdf1-119">Name</span></span>|<span data-ttu-id="afdf1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="afdf1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="afdf1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afdf1-121">Authorization</span></span>|<span data-ttu-id="afdf1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afdf1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="afdf1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afdf1-124">Content-Type</span></span>|<span data-ttu-id="afdf1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afdf1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afdf1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afdf1-127">Request body</span></span>
<span data-ttu-id="afdf1-128">В теле запроса укажу представление объекта разрешений в [JSON.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="afdf1-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="afdf1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="afdf1-129">Response</span></span>

<span data-ttu-id="afdf1-130">В случае успеха этот метод возвращает код отклика и `200 OK` объект [разрешения](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afdf1-130">If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afdf1-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="afdf1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afdf1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="afdf1-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```


### <a name="response"></a><span data-ttu-id="afdf1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="afdf1-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "2",
    "roles": ["read"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Bar App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission"
} -->
