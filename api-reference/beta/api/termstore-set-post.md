---
title: Создание набора
description: Создание нового объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ecf1327333ddd9a38d3199c01a0c6b2436eb27a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064600"
---
# <a name="create-set"></a><span data-ttu-id="669d9-103">Создание набора</span><span class="sxs-lookup"><span data-stu-id="669d9-103">Create set</span></span>
<span data-ttu-id="669d9-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="669d9-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="669d9-105">Создание нового объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="669d9-105">Create a new [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="669d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="669d9-106">Permissions</span></span>
<span data-ttu-id="669d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="669d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="669d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="669d9-109">Permission type</span></span>|<span data-ttu-id="669d9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="669d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="669d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="669d9-111">Delegated (work or school account)</span></span> |<span data-ttu-id="669d9-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="669d9-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="669d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="669d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="669d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="669d9-114">Not supported.</span></span>    |
|<span data-ttu-id="669d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="669d9-115">Application</span></span> | <span data-ttu-id="669d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="669d9-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="669d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="669d9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets
```

## <a name="request-headers"></a><span data-ttu-id="669d9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="669d9-118">Request headers</span></span>
|<span data-ttu-id="669d9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="669d9-119">Name</span></span>|<span data-ttu-id="669d9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="669d9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="669d9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="669d9-121">Authorization</span></span>|<span data-ttu-id="669d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="669d9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="669d9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="669d9-124">Content-Type</span></span>|<span data-ttu-id="669d9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="669d9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="669d9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="669d9-127">Request body</span></span>
<span data-ttu-id="669d9-128">В тексте запроса добавьте представление объекта [Set](../resources/termstore-set.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="669d9-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="669d9-129">В следующей таблице приведены свойства, необходимые при создании [набора](../resources/termstore-set.md).</span><span class="sxs-lookup"><span data-stu-id="669d9-129">The following table shows the properties that are required when you create the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="669d9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="669d9-130">Property</span></span>|<span data-ttu-id="669d9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="669d9-131">Type</span></span>|<span data-ttu-id="669d9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="669d9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="669d9-133">локализеднамес</span><span class="sxs-lookup"><span data-stu-id="669d9-133">localizedNames</span></span>|<span data-ttu-id="669d9-134">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеднаме](../resources/termstore-localizedname.md)</span><span class="sxs-lookup"><span data-stu-id="669d9-134">[microsoft.graph.termstore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="669d9-135">Имя создаваемого набора</span><span class="sxs-lookup"><span data-stu-id="669d9-135">Name of the set to be created</span></span>|
|<span data-ttu-id="669d9-136">парентграуп</span><span class="sxs-lookup"><span data-stu-id="669d9-136">parentGroup</span></span>|[<span data-ttu-id="669d9-137">Microsoft. Graph. Банк.</span><span class="sxs-lookup"><span data-stu-id="669d9-137">microsoft.graph.termstore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="669d9-138">Банк терминов — группа, в которой необходимо создать набор</span><span class="sxs-lookup"><span data-stu-id="669d9-138">termstore-group under which the set needs to be created</span></span>|



## <a name="response"></a><span data-ttu-id="669d9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="669d9-139">Response</span></span>

<span data-ttu-id="669d9-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Set](../resources/termstore-set.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="669d9-140">If successful, this method returns a `201 Created` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="669d9-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="669d9-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="669d9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="669d9-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="669d9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="669d9-143">Response</span></span>
<span data-ttu-id="669d9-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="669d9-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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


