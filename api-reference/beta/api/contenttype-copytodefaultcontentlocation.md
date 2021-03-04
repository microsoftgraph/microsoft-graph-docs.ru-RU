---
author: swapnil1993
title: 'contentType: copyToDefaultContentLocation'
description: Скопируйте файл в расположение контента по умолчанию в типе контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 913db69991d176d8537baef5abbbb8734d6c10cc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447290"
---
# <a name="contenttype-copytodefaultcontentlocation"></a><span data-ttu-id="99f3a-103">contentType: copyToDefaultContentLocation</span><span class="sxs-lookup"><span data-stu-id="99f3a-103">contentType: copyToDefaultContentLocation</span></span>
<span data-ttu-id="99f3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99f3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="99f3a-105">Скопируйте файл в расположение контента по умолчанию в [типе контента.][contentType]</span><span class="sxs-lookup"><span data-stu-id="99f3a-105">Copy a file to a default content location in a [content type][contentType].</span></span> <span data-ttu-id="99f3a-106">Затем файл может быть добавлен в качестве файла или шаблона по умолчанию с помощью операции POST.</span><span class="sxs-lookup"><span data-stu-id="99f3a-106">The file can then be added as a default file or template via a POST operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="99f3a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99f3a-107">Permissions</span></span>  

<span data-ttu-id="99f3a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="99f3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="99f3a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99f3a-110">Permission type</span></span> | <span data-ttu-id="99f3a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99f3a-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99f3a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99f3a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99f3a-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="99f3a-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="99f3a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99f3a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99f3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99f3a-115">Not supported.</span></span> |
|<span data-ttu-id="99f3a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="99f3a-116">Application</span></span> | <span data-ttu-id="99f3a-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="99f3a-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="99f3a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99f3a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http

POST /sites/id/contentTypes/id/copyToDefaultContentLocation 
```

## <a name="request-headers"></a><span data-ttu-id="99f3a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99f3a-119">Request headers</span></span>
|<span data-ttu-id="99f3a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="99f3a-120">Name</span></span>|<span data-ttu-id="99f3a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="99f3a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="99f3a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99f3a-122">Authorization</span></span>|<span data-ttu-id="99f3a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99f3a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="99f3a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99f3a-125">Content-Type</span></span>|<span data-ttu-id="99f3a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99f3a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99f3a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99f3a-128">Request body</span></span>
<span data-ttu-id="99f3a-129">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="99f3a-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="99f3a-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="99f3a-130">The following table shows the parameters that can be used with this action.</span></span>


|<span data-ttu-id="99f3a-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="99f3a-131">Parameter</span></span>|<span data-ttu-id="99f3a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="99f3a-132">Type</span></span>|<span data-ttu-id="99f3a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="99f3a-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="99f3a-134">sourceFile</span><span class="sxs-lookup"><span data-stu-id="99f3a-134">sourceFile</span></span>| [<span data-ttu-id="99f3a-135">itemReference</span><span class="sxs-lookup"><span data-stu-id="99f3a-135">itemReference</span></span>](../resources/itemreference.md) |<span data-ttu-id="99f3a-136">Метаданные о исходных файлах, которые необходимо скопировать в расположение контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f3a-136">Metadata about the source file that needs to be copied to the default content location.</span></span> <span data-ttu-id="99f3a-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99f3a-137">Required.</span></span>|
|<span data-ttu-id="99f3a-138">destinationFileName</span><span class="sxs-lookup"><span data-stu-id="99f3a-138">destinationFileName</span></span>| <span data-ttu-id="99f3a-139">string</span><span class="sxs-lookup"><span data-stu-id="99f3a-139">string</span></span> |<span data-ttu-id="99f3a-140">Имя файла назначения.</span><span class="sxs-lookup"><span data-stu-id="99f3a-140">Destination filename.</span></span> 

## <a name="response"></a><span data-ttu-id="99f3a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="99f3a-141">Response</span></span>


<span data-ttu-id="99f3a-142">В случае успешного ответа этот вызов возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="99f3a-142">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="99f3a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="99f3a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="99f3a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="99f3a-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
    "sourceFile": {
        "sharepointIds": {
            "listId": "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
            "listItemId": "2"
        }
    },
    "destinationFileName": "newname.txt"
}
```



### <a name="response"></a><span data-ttu-id="99f3a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="99f3a-145">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

  

[contentType]: ../resources/contentType.md
