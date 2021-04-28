---
title: Записи списка
description: Получите список ресурсов catalogEntry из каталога.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: c00dafaf9c6a28f5dd5c747a747ab1d8e84419a4
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068141"
---
# <a name="list-entries"></a><span data-ttu-id="8e5fc-103">Записи списка</span><span class="sxs-lookup"><span data-stu-id="8e5fc-103">List entries</span></span>
<span data-ttu-id="8e5fc-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="8e5fc-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e5fc-105">Получите список ресурсов [catalogEntry](../resources/windowsupdates-catalogentry.md) из [каталога.](../resources/windowsupdates-catalog.md)</span><span class="sxs-lookup"><span data-stu-id="8e5fc-105">Get a list of [catalogEntry](../resources/windowsupdates-catalogentry.md) resources from the [catalog](../resources/windowsupdates-catalog.md).</span></span>

<span data-ttu-id="8e5fc-106">В настоящее время эта операция возвращает записи типов [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) или [qualityUpdateCatalog,](../resources/windowsupdates-qualityupdatecatalogentry.md) унаследованных от **catalogEntry.**</span><span class="sxs-lookup"><span data-stu-id="8e5fc-106">Currently, this operation returns entries of the [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) or [qualityUpdateCatalog](../resources/windowsupdates-qualityupdatecatalogentry.md) types, inherited from **catalogEntry**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8e5fc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e5fc-107">Permissions</span></span>
<span data-ttu-id="8e5fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e5fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e5fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e5fc-110">Permission type</span></span>|<span data-ttu-id="8e5fc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e5fc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e5fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e5fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e5fc-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5fc-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="8e5fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e5fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e5fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e5fc-115">Not supported.</span></span>|
|<span data-ttu-id="8e5fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e5fc-116">Application</span></span>|<span data-ttu-id="8e5fc-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5fc-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e5fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e5fc-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/catalog/entries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e5fc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e5fc-119">Optional query parameters</span></span>
<span data-ttu-id="8e5fc-120">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="8e5fc-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="8e5fc-121">Чтобы использовать параметр запроса для свойства, которое не наследуется **из catalogEntry,** включайте полный тип ресурса для свойства.</span><span class="sxs-lookup"><span data-stu-id="8e5fc-121">To use a query parameter on a property that is not inherited from **catalogEntry**, include the full resource type for the property.</span></span> <span data-ttu-id="8e5fc-122">Например, для фильтрации свойства **версии** [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md)используйте `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version` .</span><span class="sxs-lookup"><span data-stu-id="8e5fc-122">For example, to filter on the **version** property of [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), use `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e5fc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e5fc-123">Request headers</span></span>
|<span data-ttu-id="8e5fc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8e5fc-124">Name</span></span>|<span data-ttu-id="8e5fc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8e5fc-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8e5fc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e5fc-126">Authorization</span></span>|<span data-ttu-id="8e5fc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e5fc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e5fc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e5fc-129">Request body</span></span>
<span data-ttu-id="8e5fc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e5fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e5fc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e5fc-131">Response</span></span>

<span data-ttu-id="8e5fc-132">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` объектов catalogEntry в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e5fc-132">If successful, this method returns a `200 OK` response code and a collection of catalogEntry objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e5fc-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e5fc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e5fc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e5fc-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_catalogentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries
```


### <a name="response"></a><span data-ttu-id="8e5fc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e5fc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.catalogEntry)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
      "id": "c1dec151-c151-c1de-51c1-dec151c1dec1",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "version": "String"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
      "id": "d0c03fbb-43b9-4dff-840b-974ef227384d",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "isExpeditable": true,
      "qualityUpdateClassification": "security"
    }
  ]
}
```

