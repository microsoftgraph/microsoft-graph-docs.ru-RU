---
author: swapnil1993
title: 'contentType: associateWithHubSites'
description: Связать тип контента со списком узлов.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8049eb6db5975c2e5c8600a654b6cc533124217f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447298"
---
# <a name="contenttype-associatewithhubsites"></a><span data-ttu-id="cfb7e-103">contentType: associateWithHubSites</span><span class="sxs-lookup"><span data-stu-id="cfb7e-103">contentType: associateWithHubSites</span></span>

<span data-ttu-id="cfb7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfb7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="cfb7e-105">Связывать [тип контента][contentType] со списком сайтов-концентраторов.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-105">Associate a [content type][contentType] with a list of hub sites.</span></span>

><span data-ttu-id="cfb7e-106">**Примечание:** Эта функция ограничена для клиентов с лицензией SharePoint Syntex.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-106">**Note:** This feature is limited to tenants that have a SharePoint Syntex license.</span></span>
  

## <a name="permissions"></a><span data-ttu-id="cfb7e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfb7e-107">Permissions</span></span>  

<span data-ttu-id="cfb7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cfb7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="cfb7e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfb7e-110">Permission type</span></span> | <span data-ttu-id="cfb7e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfb7e-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------
|<span data-ttu-id="cfb7e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfb7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cfb7e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="cfb7e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="cfb7e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfb7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfb7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-115">Not supported.</span></span> |
|<span data-ttu-id="cfb7e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cfb7e-116">Application</span></span> | <span data-ttu-id="cfb7e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="cfb7e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="cfb7e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfb7e-118">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/id/contentTypes/id/associateWithHubSites
```

## <a name="request-headers"></a><span data-ttu-id="cfb7e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfb7e-119">Request headers</span></span>
|<span data-ttu-id="cfb7e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cfb7e-120">Name</span></span>|<span data-ttu-id="cfb7e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb7e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cfb7e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfb7e-122">Authorization</span></span>|<span data-ttu-id="cfb7e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cfb7e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cfb7e-125">Content-Type</span></span>|<span data-ttu-id="cfb7e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfb7e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfb7e-128">Request body</span></span>
<span data-ttu-id="cfb7e-129">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="cfb7e-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cfb7e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="cfb7e-131">Parameter</span></span>|<span data-ttu-id="cfb7e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cfb7e-132">Type</span></span>|<span data-ttu-id="cfb7e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb7e-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="cfb7e-134">hubSiteUrls</span><span class="sxs-lookup"><span data-stu-id="cfb7e-134">hubSiteUrls</span></span>| <span data-ttu-id="cfb7e-135">Коллекция (строка)</span><span class="sxs-lookup"><span data-stu-id="cfb7e-135">Collection(string)</span></span> |<span data-ttu-id="cfb7e-136">Список пушечных URL-адресов для узлов, на которых необходимо применять тип контента.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-136">List of cannonical URLs to the hub sites where the content type needs to be enforced.</span></span> <span data-ttu-id="cfb7e-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-137">Required.</span></span>|
|<span data-ttu-id="cfb7e-138">propagateToExistingLists</span><span class="sxs-lookup"><span data-stu-id="cfb7e-138">propagateToExistingLists</span></span>| <span data-ttu-id="cfb7e-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfb7e-139">Boolean</span></span> |<span data-ttu-id="cfb7e-140">Если типы контента будут применяться в существующих списках на сайтах концентратора; в противном случае он будет применяться только к вновь `true` созданным спискам.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-140">If `true`, content types will be enforced on existing lists in the hub sites; otherwise, it will be applied only to newly created lists.</span></span> 

## <a name="response"></a><span data-ttu-id="cfb7e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfb7e-141">Response</span></span>

<span data-ttu-id="cfb7e-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cfb7e-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cfb7e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="cfb7e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfb7e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfb7e-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/contentTypes/id/associateWithHubSites
Content-Type: application/json

{
  "hubSiteUrls":
    [
      "https://graph.microsoft.com/beta/sites/id"
      
    ],
    "propagateToExistingLists": false
}
```



### <a name="response"></a><span data-ttu-id="cfb7e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfb7e-145">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

  

[contentType]: ../resources/contentType.md
