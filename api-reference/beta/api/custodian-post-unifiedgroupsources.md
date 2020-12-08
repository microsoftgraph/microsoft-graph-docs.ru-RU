---
title: Создание Унифиедграупсаурце
description: Создание нового объекта Унифиедграупсаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f92fa2454b7ab20946091784af11b23ef2252acc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597738"
---
# <a name="create-unifiedgroupsource"></a><span data-ttu-id="c3b6c-103">Создание Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="c3b6c-103">Create unifiedGroupSource</span></span>

<span data-ttu-id="c3b6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3b6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3b6c-105">Создание нового объекта [унифиедграупсаурце](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="c3b6c-105">Create a new [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3b6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b6c-106">Permissions</span></span>

<span data-ttu-id="c3b6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3b6c-109">Permission type</span></span>|<span data-ttu-id="c3b6c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3b6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3b6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3b6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3b6c-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c3b6c-112">User.Read</span></span>|
|<span data-ttu-id="c3b6c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3b6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3b6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-114">Not supported.</span></span>|
|<span data-ttu-id="c3b6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3b6c-115">Application</span></span>|<span data-ttu-id="c3b6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3b6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3b6c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a><span data-ttu-id="c3b6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3b6c-118">Request headers</span></span>

|<span data-ttu-id="c3b6c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c3b6c-119">Name</span></span>|<span data-ttu-id="c3b6c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b6c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3b6c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3b6c-121">Authorization</span></span>|<span data-ttu-id="c3b6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3b6c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3b6c-124">Content-Type</span></span>|<span data-ttu-id="c3b6c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3b6c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3b6c-127">Request body</span></span>

<span data-ttu-id="c3b6c-128">В тексте запроса добавьте представление объекта [унифиедграупсаурце](../resources/unifiedgroupsource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-128">In the request body, supply a JSON representation of the [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

<span data-ttu-id="c3b6c-129">В следующей таблице приведены свойства, необходимые при создании [унифиедграупсаурце](../resources/unifiedgroupsource.md).</span><span class="sxs-lookup"><span data-stu-id="c3b6c-129">The following table shows the properties that are required when you create the [unifiedGroupSource](../resources/unifiedgroupsource.md).</span></span>

|<span data-ttu-id="c3b6c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3b6c-130">Property</span></span>|<span data-ttu-id="c3b6c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3b6c-131">Type</span></span>|<span data-ttu-id="c3b6c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3b6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3b6c-133">инклудедсаурцес</span><span class="sxs-lookup"><span data-stu-id="c3b6c-133">includedSources</span></span>|<span data-ttu-id="c3b6c-134">sourceType</span><span class="sxs-lookup"><span data-stu-id="c3b6c-134">sourceType</span></span>|<span data-ttu-id="c3b6c-135">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-135">Specifies which sources are included in this group.</span></span> <span data-ttu-id="c3b6c-136">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-136">Possible values are: `mailbox`, `site`.</span></span>|
|<span data-ttu-id="c3b6c-137">group@odata. Bind</span><span class="sxs-lookup"><span data-stu-id="c3b6c-137">group@odata.bind</span></span>|<span data-ttu-id="c3b6c-138">String</span><span class="sxs-lookup"><span data-stu-id="c3b6c-138">String</span></span>|<span data-ttu-id="c3b6c-139">Идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-139">ID of the group.</span></span> <span data-ttu-id="c3b6c-140">Чтобы получить идентификатор группы, используйте операцию " [список групп](../api/group-list.md) ".</span><span class="sxs-lookup"><span data-stu-id="c3b6c-140">To get the group ID, use the [List groups](../api/group-list.md) operation.</span></span>|

## <a name="response"></a><span data-ttu-id="c3b6c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b6c-141">Response</span></span>

<span data-ttu-id="c3b6c-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унифиедграупсаурце](../resources/unifiedgroupsource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-142">If successful, this method returns a `201 Created` response code and a [unifiedGroupSource](../resources/unifiedgroupsource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3b6c-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3b6c-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3b6c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3b6c-144">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="c3b6c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3b6c-145">Response</span></span>

<span data-ttu-id="c3b6c-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3b6c-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
