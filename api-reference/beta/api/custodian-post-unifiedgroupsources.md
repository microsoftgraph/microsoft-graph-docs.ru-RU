---
title: Создание unifiedGroupSource
description: Создание объекта unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 61e7ff3aef7c4a94b0a0efcbc0f012b7eda0b604
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872550"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="b450a-103">Создание unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="b450a-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="b450a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b450a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b450a-105">Создание объекта [unifiedGroupSource.](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="b450a-105">Create a new [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b450a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b450a-106">Permissions</span></span>

<span data-ttu-id="b450a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b450a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b450a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b450a-109">Permission type</span></span>|<span data-ttu-id="b450a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b450a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b450a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b450a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b450a-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="b450a-112">User.Read</span></span>|
|<span data-ttu-id="b450a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b450a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b450a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b450a-114">Not supported.</span></span>|
|<span data-ttu-id="b450a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b450a-115">Application</span></span>|<span data-ttu-id="b450a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b450a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b450a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b450a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="b450a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b450a-118">Request headers</span></span>

|<span data-ttu-id="b450a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b450a-119">Name</span></span>|<span data-ttu-id="b450a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b450a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b450a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b450a-121">Authorization</span></span>|<span data-ttu-id="b450a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b450a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b450a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b450a-124">Content-Type</span></span>|<span data-ttu-id="b450a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b450a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b450a-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="b450a-127">Request body</span></span>

<span data-ttu-id="b450a-128">В теле запроса укажу представление объекта [unifiedGroupSource](../resources/unifiedgroupsource.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="b450a-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="b450a-129">В следующей таблице показаны свойства, необходимые при создании [unifiedGroupSource.](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="b450a-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/unifiedgroupsource.md).</span></span>

|<span data-ttu-id="b450a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b450a-130">Property</span></span>|<span data-ttu-id="b450a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b450a-131">Type</span></span>|<span data-ttu-id="b450a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b450a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b450a-133">includedSources</span><span class="sxs-lookup"><span data-stu-id="b450a-133">includedSources</span></span>|<span data-ttu-id="b450a-134">sourceType</span><span class="sxs-lookup"><span data-stu-id="b450a-134">sourceType</span></span>|<span data-ttu-id="b450a-135">Указывает источники, включенные в эту группу.</span><span class="sxs-lookup"><span data-stu-id="b450a-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="b450a-136">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="b450a-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="b450a-137">group@odata.bind</span><span class="sxs-lookup"><span data-stu-id="b450a-137">group@odata.bind</span></span>|<span data-ttu-id="b450a-138">String</span><span class="sxs-lookup"><span data-stu-id="b450a-138">String</span></span>|<span data-ttu-id="b450a-139">ИД группы.</span><span class="sxs-lookup"><span data-stu-id="b450a-139">ID of the group.</span></span> <span data-ttu-id="b450a-140">Чтобы получить ИД группы, используйте операцию ["Группы](../api/group-list.md) списков".</span><span class="sxs-lookup"><span data-stu-id="b450a-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="b450a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b450a-141">Response</span></span>

<span data-ttu-id="b450a-142">В случае успеха этот метод возвращает код отклика и объект `201 Created` [unifiedGroupSource](../resources/unifiedgroupsource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b450a-142">If successful, this method returns a `201 Created` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b450a-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="b450a-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b450a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b450a-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b450a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b450a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```
# <a name="c"></a>[<span data-ttu-id="b450a-146">C#</span><span class="sxs-lookup"><span data-stu-id="b450a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedgroupsource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b450a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b450a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedgroupsource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b450a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b450a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedgroupsource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b450a-149">Java</span><span class="sxs-lookup"><span data-stu-id="b450a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedgroupsource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b450a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b450a-150">Response</span></span>

<span data-ttu-id="b450a-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b450a-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site",
  "id": "14202dd90a1f4ccc84929586326c7104",
  "displayName": "SFA Videos",
  "createdDateTime": "2020-03-13T22:38:00.8985662Z",
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Megan Bowen"
      }
  }
}
```
