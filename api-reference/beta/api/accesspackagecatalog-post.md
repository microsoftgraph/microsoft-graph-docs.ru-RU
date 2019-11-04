---
title: Создание Акцесспаккажекаталог
description: Создание нового Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f0683a1160b9deaf30b4ebc782b405417ef4db
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936084"
---
# <a name="create-accesspackagecatalog"></a><span data-ttu-id="b97b3-103">Создание Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="b97b3-103">Create accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b97b3-104">Создание нового объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="b97b3-104">Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b97b3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b97b3-105">Permissions</span></span>

<span data-ttu-id="b97b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b97b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b97b3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b97b3-108">Permission type</span></span>                        | <span data-ttu-id="b97b3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b97b3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b97b3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b97b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b97b3-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b97b3-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b97b3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b97b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b97b3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b97b3-113">Not supported.</span></span> |
| <span data-ttu-id="b97b3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b97b3-114">Application</span></span>                            | <span data-ttu-id="b97b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b97b3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b97b3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b97b3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a><span data-ttu-id="b97b3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b97b3-117">Request headers</span></span>

| <span data-ttu-id="b97b3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b97b3-118">Name</span></span>          | <span data-ttu-id="b97b3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b97b3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b97b3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b97b3-120">Authorization</span></span> | <span data-ttu-id="b97b3-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="b97b3-121">Bearer \{token\}.</span></span> <span data-ttu-id="b97b3-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b97b3-122">Required.</span></span> |
| <span data-ttu-id="b97b3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b97b3-123">Content-Type</span></span>  | <span data-ttu-id="b97b3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b97b3-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b97b3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b97b3-125">Request body</span></span>

<span data-ttu-id="b97b3-126">В тексте запроса добавьте представление объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b97b3-126">In the request body, supply a JSON representation of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>  <span data-ttu-id="b97b3-127">Включите свойства **DisplayName**, **Description**и **исекстерналливисибле** .</span><span class="sxs-lookup"><span data-stu-id="b97b3-127">Include the **displayname**, **description**, and **isExternallyVisible** properties.</span></span>

## <a name="response"></a><span data-ttu-id="b97b3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b97b3-128">Response</span></span>

<span data-ttu-id="b97b3-129">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b97b3-129">If successful, this method returns a 200-series response code and a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b97b3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b97b3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b97b3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b97b3-131">Request</span></span>

<span data-ttu-id="b97b3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b97b3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
Content-type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "isExternallyVisible": true
}
```

### <a name="response"></a><span data-ttu-id="b97b3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b97b3-133">Response</span></span>

<span data-ttu-id="b97b3-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b97b3-134">The following is an example of the response.</span></span>

> <span data-ttu-id="b97b3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b97b3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "UserManaged",
  "catalogStatus": "Published",
  "isExternallyVisible": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
