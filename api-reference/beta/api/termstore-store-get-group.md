---
title: Вывод группы
description: Чтение свойств и связей объекта Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2423e4a03a325d8873dc0e6ebdaf7038cad88497
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539444"
---
# <a name="get-group"></a><span data-ttu-id="62187-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="62187-103">Get group</span></span>
<span data-ttu-id="62187-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="62187-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62187-105">Чтение свойств и связей объекта [Group](../resources/termstore-group.md) .</span><span class="sxs-lookup"><span data-stu-id="62187-105">Read the properties and relationships of a [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62187-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62187-106">Permissions</span></span>
<span data-ttu-id="62187-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62187-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62187-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62187-109">Permission type</span></span>|<span data-ttu-id="62187-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62187-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62187-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62187-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62187-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="62187-112">TermStore.Read.All,TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="62187-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62187-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62187-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62187-114">Not supported.</span></span>    |
|<span data-ttu-id="62187-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62187-115">Application</span></span> | <span data-ttu-id="62187-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62187-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="62187-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62187-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="62187-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62187-118">Request headers</span></span>
|<span data-ttu-id="62187-119">Имя</span><span class="sxs-lookup"><span data-stu-id="62187-119">Name</span></span>|<span data-ttu-id="62187-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62187-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62187-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62187-121">Authorization</span></span>|<span data-ttu-id="62187-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62187-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62187-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62187-124">Request body</span></span>
<span data-ttu-id="62187-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62187-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62187-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="62187-126">Response</span></span>

<span data-ttu-id="62187-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/termstore-group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="62187-127">If successful, this method returns a `200 OK` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62187-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="62187-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62187-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="62187-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}
```


### <a name="response"></a><span data-ttu-id="62187-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="62187-130">Response</span></span>

<span data-ttu-id="62187-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62187-131">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "id": "1FFD3F87-9464-488A-A0EC-8FB90911182C",
  "displayName": "myGroup"  
}
```

[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termGroup",
  "suppressions": [
  ]
}
-->
