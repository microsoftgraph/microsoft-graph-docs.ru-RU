---
title: Создание разрешения
description: Создание объекта разрешений.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6952931c2925e0de229d93d47b62d77e702c1873
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160857"
---
# <a name="create-permission"></a><span data-ttu-id="15d40-103">Создание разрешения</span><span class="sxs-lookup"><span data-stu-id="15d40-103">Create permission</span></span>
<span data-ttu-id="15d40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15d40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15d40-105">Создание объекта [разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="15d40-105">Create a new [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="15d40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15d40-106">Permissions</span></span>
<span data-ttu-id="15d40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15d40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15d40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15d40-109">Permission type</span></span>                        | <span data-ttu-id="15d40-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15d40-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="15d40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15d40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="15d40-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15d40-112">Not supported.</span></span>
|<span data-ttu-id="15d40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15d40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15d40-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15d40-114">Not supported.</span></span>
|<span data-ttu-id="15d40-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15d40-115">Application</span></span>                            | <span data-ttu-id="15d40-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="15d40-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="15d40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15d40-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="15d40-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15d40-118">Request headers</span></span>
|<span data-ttu-id="15d40-119">Имя</span><span class="sxs-lookup"><span data-stu-id="15d40-119">Name</span></span>|<span data-ttu-id="15d40-120">Описание</span><span class="sxs-lookup"><span data-stu-id="15d40-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="15d40-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15d40-121">Authorization</span></span>|<span data-ttu-id="15d40-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15d40-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="15d40-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15d40-124">Content-Type</span></span>|<span data-ttu-id="15d40-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15d40-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15d40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15d40-127">Request body</span></span>
<span data-ttu-id="15d40-128">В теле запроса укажу представление объекта разрешений в [JSON.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="15d40-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="15d40-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="15d40-129">Response</span></span>

<span data-ttu-id="15d40-130">В случае успеха этот метод возвращает код отклика и `201 Created` объект [разрешения](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15d40-130">If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15d40-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="15d40-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15d40-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="15d40-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_permission_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{sitesId}/permissions
Content-Type: application/json

{
  "roles": ["write"],
  "grantedToIdentities": [{
    "application": {
      "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      "displayName": "Foo App"
    }
  }]
}
```


### <a name="response"></a><span data-ttu-id="15d40-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="15d40-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "1",
    "roles": ["write"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Foo App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Create site permissions"
} -->
