---
title: Создание тега
description: Создайте новый объект тегов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ee08824511ffd3f32b78d5c04726686eee4d4dd4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447113"
---
# <a name="create-tag"></a><span data-ttu-id="752c3-103">Создание тега</span><span class="sxs-lookup"><span data-stu-id="752c3-103">Create tag</span></span>

<span data-ttu-id="752c3-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="752c3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="752c3-105">Создайте новый тег для указанного случая.</span><span class="sxs-lookup"><span data-stu-id="752c3-105">Create a new tag for the specified case.</span></span>  <span data-ttu-id="752c3-106">Теги используются в наборах обзоров при просмотре контента.</span><span class="sxs-lookup"><span data-stu-id="752c3-106">The tags are used in review sets while reviewing content.</span></span>

## <a name="permissions"></a><span data-ttu-id="752c3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="752c3-107">Permissions</span></span>

<span data-ttu-id="752c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="752c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="752c3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="752c3-110">Permission type</span></span>|<span data-ttu-id="752c3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="752c3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="752c3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="752c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="752c3-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="752c3-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="752c3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="752c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="752c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="752c3-115">Not supported.</span></span>|
|<span data-ttu-id="752c3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="752c3-116">Application</span></span>|<span data-ttu-id="752c3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="752c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="752c3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="752c3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="request-headers"></a><span data-ttu-id="752c3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="752c3-119">Request headers</span></span>

|<span data-ttu-id="752c3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="752c3-120">Name</span></span>|<span data-ttu-id="752c3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="752c3-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="752c3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="752c3-122">Authorization</span></span>|<span data-ttu-id="752c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="752c3-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="752c3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="752c3-125">Content-Type</span></span>|<span data-ttu-id="752c3-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="752c3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="752c3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="752c3-128">Request body</span></span>

<span data-ttu-id="752c3-129">В теле запроса поставляем представление JSON объекта [тегов.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="752c3-129">In the request body, supply a JSON representation of the [tag](../resources/ediscovery-tag.md) object.</span></span>

<span data-ttu-id="752c3-130">В следующей таблице показаны свойства, необходимые при создании [тега.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="752c3-130">The following table shows the properties that are required when you create the [tag](../resources/ediscovery-tag.md).</span></span>

|<span data-ttu-id="752c3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="752c3-131">Property</span></span>|<span data-ttu-id="752c3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="752c3-132">Type</span></span>|<span data-ttu-id="752c3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="752c3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="752c3-134">childSelectability</span><span class="sxs-lookup"><span data-stu-id="752c3-134">childSelectability</span></span>|[<span data-ttu-id="752c3-135">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="752c3-135">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="752c3-136">Указывает, можно ли связывать один или несколько детских тегов с документом.</span><span class="sxs-lookup"><span data-stu-id="752c3-136">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="752c3-137">Возможные значения: `One`, `Many`.</span><span class="sxs-lookup"><span data-stu-id="752c3-137">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="752c3-138">Это значение контролирует, представляет ли UX теги в качестве почтовых ящиков или группы кнопок радио.</span><span class="sxs-lookup"><span data-stu-id="752c3-138">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span> <span data-ttu-id="752c3-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="752c3-139">Required.</span></span>|
|<span data-ttu-id="752c3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="752c3-140">displayName</span></span>|<span data-ttu-id="752c3-141">String</span><span class="sxs-lookup"><span data-stu-id="752c3-141">String</span></span>|<span data-ttu-id="752c3-142">Отображение имени тега.</span><span class="sxs-lookup"><span data-stu-id="752c3-142">Display name of the tag.</span></span> <span data-ttu-id="752c3-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="752c3-143">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="752c3-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="752c3-144">Response</span></span>

<span data-ttu-id="752c3-145">В случае успешного решения этот метод возвращает код ответа и `201 Created` [объект microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="752c3-145">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="752c3-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="752c3-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="752c3-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="752c3-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tag_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
Content-Type: application/json
Content-length: 235

{
  "displayName":"Privileged",
  "description":"The document is privileged",
  "parent@odata.bind":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}
```

### <a name="response"></a><span data-ttu-id="752c3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="752c3-148">Response</span></span>

<span data-ttu-id="752c3-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="752c3-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/$entity",
    "displayName": "Privileged",
    "description": "The document is privileged",
    "lastModifiedDateTime": "2021-01-12T01:01:09.0419153Z",
    "childSelectability": "One",
    "id": "0825ef81ade74095a3b3154a3c434c3e",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
