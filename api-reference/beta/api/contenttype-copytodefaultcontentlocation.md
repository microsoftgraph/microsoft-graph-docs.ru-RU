---
author: swapnil1993
title: 'contentType: copyToDefaultContentLocation'
description: Скопируйте файл в расположение контента по умолчанию в типе контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: afe4a5aebe4e19dd3957e0be0cca334a33035981
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201990"
---
# <a name="contenttype-copytodefaultcontentlocation"></a><span data-ttu-id="197e7-103">contentType: copyToDefaultContentLocation</span><span class="sxs-lookup"><span data-stu-id="197e7-103">contentType: copyToDefaultContentLocation</span></span>
<span data-ttu-id="197e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="197e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="197e7-105">Скопируйте файл в расположение контента по умолчанию в [типе контента.][contentType]</span><span class="sxs-lookup"><span data-stu-id="197e7-105">Copy a file to a default content location in a [content type][contentType].</span></span> <span data-ttu-id="197e7-106">Затем файл может быть добавлен в качестве файла или шаблона по умолчанию с помощью операции POST.</span><span class="sxs-lookup"><span data-stu-id="197e7-106">The file can then be added as a default file or template via a POST operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="197e7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="197e7-107">Permissions</span></span>  

<span data-ttu-id="197e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="197e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="197e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="197e7-110">Permission type</span></span> | <span data-ttu-id="197e7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="197e7-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="197e7-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="197e7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="197e7-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="197e7-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="197e7-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="197e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="197e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="197e7-115">Not supported.</span></span> |
|<span data-ttu-id="197e7-116">Application</span><span class="sxs-lookup"><span data-stu-id="197e7-116">Application</span></span> | <span data-ttu-id="197e7-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="197e7-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="197e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="197e7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /sites/id/contentTypes/id/copyToDefaultContentLocation 
```

## <a name="request-headers"></a><span data-ttu-id="197e7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="197e7-119">Request headers</span></span>
|<span data-ttu-id="197e7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="197e7-120">Name</span></span>|<span data-ttu-id="197e7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="197e7-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="197e7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="197e7-122">Authorization</span></span>|<span data-ttu-id="197e7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="197e7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="197e7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="197e7-125">Content-Type</span></span>|<span data-ttu-id="197e7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="197e7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="197e7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="197e7-128">Request body</span></span>
<span data-ttu-id="197e7-129">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="197e7-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="197e7-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="197e7-130">The following table shows the parameters that can be used with this action.</span></span>


|<span data-ttu-id="197e7-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="197e7-131">Parameter</span></span>|<span data-ttu-id="197e7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="197e7-132">Type</span></span>|<span data-ttu-id="197e7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="197e7-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="197e7-134">sourceFile</span><span class="sxs-lookup"><span data-stu-id="197e7-134">sourceFile</span></span>| [<span data-ttu-id="197e7-135">itemReference</span><span class="sxs-lookup"><span data-stu-id="197e7-135">itemReference</span></span>](../resources/itemreference.md) |<span data-ttu-id="197e7-136">Метаданные о исходных файлах, которые необходимо скопировать в расположение контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="197e7-136">Metadata about the source file that needs to be copied to the default content location.</span></span> <span data-ttu-id="197e7-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="197e7-137">Required.</span></span>|
|<span data-ttu-id="197e7-138">destinationFileName</span><span class="sxs-lookup"><span data-stu-id="197e7-138">destinationFileName</span></span>| <span data-ttu-id="197e7-139">строка</span><span class="sxs-lookup"><span data-stu-id="197e7-139">string</span></span> |<span data-ttu-id="197e7-140">Имя файла назначения.</span><span class="sxs-lookup"><span data-stu-id="197e7-140">Destination filename.</span></span> 

## <a name="response"></a><span data-ttu-id="197e7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="197e7-141">Response</span></span>


<span data-ttu-id="197e7-142">В случае успешного ответа этот вызов возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="197e7-142">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="197e7-143">Пример</span><span class="sxs-lookup"><span data-stu-id="197e7-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="197e7-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="197e7-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="197e7-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="197e7-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
   "sourceFile":{
      "sharepointIds":{
         "listId":"e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
         "listItemId":"2"
      }
   },
   "destinationFileName":"newname.txt"
}
```
# <a name="c"></a>[<span data-ttu-id="197e7-146">C#</span><span class="sxs-lookup"><span data-stu-id="197e7-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-copytodefaultcontentlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="197e7-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="197e7-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-copytodefaultcontentlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="197e7-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="197e7-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-copytodefaultcontentlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="197e7-149">Java</span><span class="sxs-lookup"><span data-stu-id="197e7-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-copytodefaultcontentlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="197e7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="197e7-150">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
