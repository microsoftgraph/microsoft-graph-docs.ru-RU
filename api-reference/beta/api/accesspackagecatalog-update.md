---
title: Обновление Акцесспаккажекаталог
description: Обновление свойств объекта Акцесспаккажекаталог.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3145fcd5fda95bb9c76763bf804ef3a4f4cce7d7
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757482"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="951fa-103">Обновление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="951fa-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="951fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="951fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="951fa-105">Обновление существующего объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.</span><span class="sxs-lookup"><span data-stu-id="951fa-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="951fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="951fa-106">Permissions</span></span>
<span data-ttu-id="951fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="951fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="951fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="951fa-109">Permission type</span></span>|<span data-ttu-id="951fa-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="951fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="951fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="951fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="951fa-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="951fa-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="951fa-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="951fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="951fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="951fa-114">Not supported.</span></span> |
|<span data-ttu-id="951fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="951fa-115">Application</span></span>                            | <span data-ttu-id="951fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="951fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="951fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="951fa-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="951fa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="951fa-118">Request headers</span></span>
|<span data-ttu-id="951fa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="951fa-119">Name</span></span>|<span data-ttu-id="951fa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="951fa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="951fa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="951fa-121">Authorization</span></span>|<span data-ttu-id="951fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="951fa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="951fa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="951fa-124">Content-Type</span></span>|<span data-ttu-id="951fa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="951fa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="951fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="951fa-127">Request body</span></span>
<span data-ttu-id="951fa-128">В тексте запроса добавьте представление объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="951fa-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="951fa-129">В следующей таблице приведены свойства, необходимые при обновлении [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="951fa-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="951fa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="951fa-130">Property</span></span>|<span data-ttu-id="951fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="951fa-131">Type</span></span>|<span data-ttu-id="951fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="951fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="951fa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="951fa-133">displayName</span></span>|<span data-ttu-id="951fa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="951fa-134">String</span></span>|<span data-ttu-id="951fa-135">Имя каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="951fa-135">The access package catalog name.</span></span>|
|<span data-ttu-id="951fa-136">description</span><span class="sxs-lookup"><span data-stu-id="951fa-136">description</span></span>|<span data-ttu-id="951fa-137">String</span><span class="sxs-lookup"><span data-stu-id="951fa-137">String</span></span>|<span data-ttu-id="951fa-138">Описание каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="951fa-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="951fa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="951fa-139">Response</span></span>
<span data-ttu-id="951fa-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="951fa-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="951fa-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="951fa-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="951fa-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="951fa-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
Content-Type: application/json
Content-length: 39

{
  "displayName":"Catalog One"
}
```


### <a name="response"></a><span data-ttu-id="951fa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="951fa-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
