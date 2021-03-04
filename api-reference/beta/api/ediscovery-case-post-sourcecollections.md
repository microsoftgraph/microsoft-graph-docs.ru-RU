---
title: Создание sourceCollection
description: Создайте новый объект sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 69476c91acffc6d0a1edc8a18cc4208c5239fa26
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447119"
---
# <a name="create-sourcecollection"></a><span data-ttu-id="a91c3-103">Создание sourceCollection</span><span class="sxs-lookup"><span data-stu-id="a91c3-103">Create sourceCollection</span></span>

<span data-ttu-id="a91c3-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a91c3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91c3-105">Создайте новый [объект sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a91c3-105">Create a new [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a91c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a91c3-106">Permissions</span></span>

<span data-ttu-id="a91c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a91c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a91c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a91c3-109">Permission type</span></span>|<span data-ttu-id="a91c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a91c3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a91c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a91c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a91c3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91c3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a91c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a91c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a91c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91c3-114">Not supported.</span></span>|
|<span data-ttu-id="a91c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a91c3-115">Application</span></span>|<span data-ttu-id="a91c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a91c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a91c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="request-headers"></a><span data-ttu-id="a91c3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a91c3-118">Request headers</span></span>

|<span data-ttu-id="a91c3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a91c3-119">Name</span></span>|<span data-ttu-id="a91c3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a91c3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a91c3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a91c3-121">Authorization</span></span>|<span data-ttu-id="a91c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a91c3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a91c3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a91c3-124">Content-Type</span></span>|<span data-ttu-id="a91c3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a91c3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a91c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a91c3-127">Request body</span></span>

<span data-ttu-id="a91c3-128">В теле запроса поставляем представление JSON объекта [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a91c3-128">In the request body, supply a JSON representation of the [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

<span data-ttu-id="a91c3-129">В следующей таблице показаны свойства, необходимые при создании [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="a91c3-129">The following table shows the properties that are required when you create the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>

|<span data-ttu-id="a91c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a91c3-130">Property</span></span>|<span data-ttu-id="a91c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a91c3-131">Type</span></span>|<span data-ttu-id="a91c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a91c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a91c3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a91c3-133">displayName</span></span>|<span data-ttu-id="a91c3-134">String</span><span class="sxs-lookup"><span data-stu-id="a91c3-134">String</span></span>|<span data-ttu-id="a91c3-135">Имя отображения **sourceCollection**</span><span class="sxs-lookup"><span data-stu-id="a91c3-135">The display name of the **sourceCollection**</span></span>|
|<span data-ttu-id="a91c3-136">custodianSources</span><span class="sxs-lookup"><span data-stu-id="a91c3-136">custodianSources</span></span>|<span data-ttu-id="a91c3-137">[коллекция microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="a91c3-137">[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection</span></span>|<span data-ttu-id="a91c3-138">Источники хранителя, которые необходимо включить в этот поиск.</span><span class="sxs-lookup"><span data-stu-id="a91c3-138">The custodian sources to include in this search.</span></span> <span data-ttu-id="a91c3-139">URL-адрес можно получить с [сайта-хранителяSources,](../api/ediscovery-custodian-list-sitesources.md) [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)или [userSources](../api/ediscovery-custodian-list-usersources.md) плюс ID источника.</span><span class="sxs-lookup"><span data-stu-id="a91c3-139">You can get the URL from from custodian [siteSources](../api/ediscovery-custodian-list-sitesources.md), [unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md), or [userSources](../api/ediscovery-custodian-list-usersources.md) plus the ID of the source.</span></span> <span data-ttu-id="a91c3-140">**Примечание:** При создании коллекции исходных данных требуется один хранитель или указать источник клиента.</span><span class="sxs-lookup"><span data-stu-id="a91c3-140">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span> |
|<span data-ttu-id="a91c3-141">tenantSources</span><span class="sxs-lookup"><span data-stu-id="a91c3-141">tenantSources</span></span>|<span data-ttu-id="a91c3-142">microsoft.graph.ediscovery.tenantSources</span><span class="sxs-lookup"><span data-stu-id="a91c3-142">microsoft.graph.ediscovery.tenantSources</span></span>|<span data-ttu-id="a91c3-143">При указании коллекция будет охватывать всю службу для всей рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="a91c3-143">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="a91c3-144">Возможные значения: `allMailboxes`, `allSites`.</span><span class="sxs-lookup"><span data-stu-id="a91c3-144">Possible values are: `allMailboxes`, `allSites`.</span></span> <span data-ttu-id="a91c3-145">**Примечание:** При создании коллекции исходных данных требуется один хранитель или указать источник клиента.</span><span class="sxs-lookup"><span data-stu-id="a91c3-145">**Note:** Either one custodian or specifying tenant source is required when creating a source collection.</span></span>|

## <a name="response"></a><span data-ttu-id="a91c3-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91c3-146">Response</span></span>

<span data-ttu-id="a91c3-147">В случае успеха этот метод возвращает код отклика и `201 Created` [объект microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a91c3-147">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a91c3-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="a91c3-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a91c3-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a91c3-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_sourcecollection_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections
Content-Type: application/json
Content-length: 272

{
    "displayName": "Quarterly Financials search",
    "contentQuery": "subject:'Quarterly Financials'",
    "custodianSources@odata.bind": [
        "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735"
    ]
}
```

### <a name="response"></a><span data-ttu-id="a91c3-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a91c3-150">Response</span></span>

<span data-ttu-id="a91c3-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a91c3-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "tenantSources": "none",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    }
}
```
