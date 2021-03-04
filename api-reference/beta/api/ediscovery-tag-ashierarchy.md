---
title: 'тег: asHierarchy'
description: Верни список тегов в иерархической форме.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7f4de1ad20f683286f177e90386511118bb9acb9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446861"
---
# <a name="tag-ashierarchy"></a><span data-ttu-id="a5db6-103">тег: asHierarchy</span><span class="sxs-lookup"><span data-stu-id="a5db6-103">tag: asHierarchy</span></span>

<span data-ttu-id="a5db6-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a5db6-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5db6-105">Возвращение списка объектов [тегов](../resources/ediscovery-tag.md) в иерархической форме</span><span class="sxs-lookup"><span data-stu-id="a5db6-105">Return a list of [tag](../resources/ediscovery-tag.md) objects in hierarchial form</span></span>

## <a name="permissions"></a><span data-ttu-id="a5db6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5db6-106">Permissions</span></span>

<span data-ttu-id="a5db6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5db6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5db6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5db6-109">Permission type</span></span>|<span data-ttu-id="a5db6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5db6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5db6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5db6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5db6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5db6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a5db6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5db6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5db6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5db6-114">Not supported.</span></span>|
|<span data-ttu-id="a5db6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5db6-115">Application</span></span>|<span data-ttu-id="a5db6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5db6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5db6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5db6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/asHierarchy
```

## <a name="request-headers"></a><span data-ttu-id="a5db6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5db6-118">Request headers</span></span>

|<span data-ttu-id="a5db6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a5db6-119">Name</span></span>|<span data-ttu-id="a5db6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a5db6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5db6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5db6-121">Authorization</span></span>|<span data-ttu-id="a5db6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5db6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5db6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5db6-124">Request body</span></span>

<span data-ttu-id="a5db6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5db6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5db6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5db6-126">Response</span></span>

<span data-ttu-id="a5db6-127">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5db6-127">If successful, this function returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5db6-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5db6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5db6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5db6-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "tag_ashierarchy"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/asHierarchy
```

### <a name="response"></a><span data-ttu-id="a5db6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5db6-130">Response</span></span>

<span data-ttu-id="a5db6-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5db6-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.tag)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.tag",
      "id": "String (identifier)",
      "displayName": "String",
      "description": "String",
      "childSelectability": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```
