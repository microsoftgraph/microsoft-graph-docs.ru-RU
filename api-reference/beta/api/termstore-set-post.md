---
title: Создание набора
description: Создание объекта set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: c81ab668593b3650dd55de6bd933eef719d8ae7d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873719"
---
# <a name="create-set"></a><span data-ttu-id="04868-103">Создание набора</span><span class="sxs-lookup"><span data-stu-id="04868-103">Create set</span></span>
<span data-ttu-id="04868-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="04868-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04868-105">Создание объекта [set.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="04868-105">Create a new [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04868-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04868-106">Permissions</span></span>
<span data-ttu-id="04868-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04868-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04868-109">Permission type</span></span>|<span data-ttu-id="04868-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04868-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04868-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04868-111">Delegated (work or school account)</span></span> |<span data-ttu-id="04868-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04868-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="04868-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04868-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04868-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04868-114">Not supported.</span></span>    |
|<span data-ttu-id="04868-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04868-115">Application</span></span> | <span data-ttu-id="04868-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04868-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="04868-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04868-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets
```

## <a name="request-headers"></a><span data-ttu-id="04868-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04868-118">Request headers</span></span>
|<span data-ttu-id="04868-119">Имя</span><span class="sxs-lookup"><span data-stu-id="04868-119">Name</span></span>|<span data-ttu-id="04868-120">Описание</span><span class="sxs-lookup"><span data-stu-id="04868-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04868-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04868-121">Authorization</span></span>|<span data-ttu-id="04868-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04868-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04868-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04868-124">Content-Type</span></span>|<span data-ttu-id="04868-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04868-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04868-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="04868-127">Request body</span></span>
<span data-ttu-id="04868-128">В теле запроса укажу представление объекта [set](../resources/termstore-set.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="04868-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="04868-129">В следующей таблице показаны свойства, необходимые при создании [набора.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="04868-129">The following table shows the properties that are required when you create the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="04868-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04868-130">Property</span></span>|<span data-ttu-id="04868-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04868-131">Type</span></span>|<span data-ttu-id="04868-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04868-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04868-133">localizedNames</span><span class="sxs-lookup"><span data-stu-id="04868-133">localizedNames</span></span>|<span data-ttu-id="04868-134">[Коллекция microsoft.graph.termstore.localizedName](../resources/termstore-localizedname.md)</span><span class="sxs-lookup"><span data-stu-id="04868-134">[microsoft.graph.termstore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="04868-135">Имя создаемого набора</span><span class="sxs-lookup"><span data-stu-id="04868-135">Name of the set to be created</span></span>|
|<span data-ttu-id="04868-136">parentGroup</span><span class="sxs-lookup"><span data-stu-id="04868-136">parentGroup</span></span>|[<span data-ttu-id="04868-137">microsoft.graph.termstore.group</span><span class="sxs-lookup"><span data-stu-id="04868-137">microsoft.graph.termstore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="04868-138">termstore-group, в которой необходимо создать набор</span><span class="sxs-lookup"><span data-stu-id="04868-138">termstore-group under which the set needs to be created</span></span>|



## <a name="response"></a><span data-ttu-id="04868-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="04868-139">Response</span></span>

<span data-ttu-id="04868-140">В случае успеха этот метод возвращает код отклика и `201 Created` [объект set](../resources/termstore-set.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04868-140">If successful, this method returns a `201 Created` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04868-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="04868-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04868-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="04868-142">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/termStore/sets
Content-Type: application/json
Content-length: 288

{
  "@odata.type": "#microsoft.graph.termStore.set",
  "parentGroup":{
      "id": "fc733b51-10f1-40fd-b784-dc6d1e42804b"
   },
   "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


### <a name="response"></a><span data-ttu-id="04868-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="04868-143">Response</span></span>
<span data-ttu-id="04868-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04868-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.set"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termSet",
  "suppressions": [
  ]
}
-->


