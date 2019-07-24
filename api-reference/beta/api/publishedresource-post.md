---
title: Создание Публишедресаурце
description: Создание нового объекта **публишедресаурце** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8823d80a3786ea8a8d3b1b3e1f7a1ef467e7384c
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840977"
---
# <a name="create-publishedresource"></a><span data-ttu-id="2f614-103">Создание Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="2f614-103">Create publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f614-104">Создание нового объекта [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="2f614-104">Create a new [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f614-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f614-105">Permissions</span></span>

<span data-ttu-id="2f614-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f614-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f614-108">Permission type</span></span>                        | <span data-ttu-id="2f614-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f614-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f614-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f614-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f614-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2f614-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2f614-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f614-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f614-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f614-113">Not supported.</span></span> |
| <span data-ttu-id="2f614-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f614-114">Application</span></span>                            | <span data-ttu-id="2f614-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f614-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f614-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f614-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="request-headers"></a><span data-ttu-id="2f614-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f614-117">Request headers</span></span>

| <span data-ttu-id="2f614-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2f614-118">Name</span></span>      |<span data-ttu-id="2f614-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2f614-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f614-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f614-120">Authorization</span></span> | <span data-ttu-id="2f614-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2f614-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f614-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f614-122">Request body</span></span>

<span data-ttu-id="2f614-123">В тексте запроса добавьте представление объекта [публишедресаурце](../resources/publishedresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f614-123">In the request body, supply a JSON representation of a [publishedResource](../resources/publishedresource.md) object.</span></span>

<span data-ttu-id="2f614-124">Укажите значения для следующих свойств.</span><span class="sxs-lookup"><span data-stu-id="2f614-124">Supply the values for the following properties.</span></span>

| <span data-ttu-id="2f614-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f614-125">Property</span></span>     | <span data-ttu-id="2f614-126">Тип</span><span class="sxs-lookup"><span data-stu-id="2f614-126">Type</span></span>        | <span data-ttu-id="2f614-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2f614-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f614-128">displayName</span><span class="sxs-lookup"><span data-stu-id="2f614-128">displayName</span></span>|<span data-ttu-id="2f614-129">String</span><span class="sxs-lookup"><span data-stu-id="2f614-129">String</span></span>|<span data-ttu-id="2f614-130">Отображаемое имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="2f614-130">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="2f614-131">resourceName</span><span class="sxs-lookup"><span data-stu-id="2f614-131">resourceName</span></span>|<span data-ttu-id="2f614-132">String</span><span class="sxs-lookup"><span data-stu-id="2f614-132">String</span></span>|<span data-ttu-id="2f614-133">Имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="2f614-133">Name of the publishedResource.</span></span>|

## <a name="response"></a><span data-ttu-id="2f614-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f614-134">Response</span></span>

<span data-ttu-id="2f614-135">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f614-135">If successful, this method returns a `201 Created` response code and [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f614-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f614-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f614-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f614-137">Request</span></span>

<span data-ttu-id="2f614-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f614-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_publishedresource_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources
Content-Type: application/json

{
    "displayName": "New provisioning",
    "resourceName": "domain1.contoso.com"
}
```

### <a name="response"></a><span data-ttu-id="2f614-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f614-139">Response</span></span>

<span data-ttu-id="2f614-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f614-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2f614-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f614-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 201 Created

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "publishingType": "provisioning",
    "displayName": "New provisionin",
    "resourceName": "domain1.contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
