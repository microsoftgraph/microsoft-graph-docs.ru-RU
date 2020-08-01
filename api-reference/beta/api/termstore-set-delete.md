---
title: Удаление набора
description: Удаление объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 83b48322c28330d22047a15cc488d276281fcc71
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539404"
---
# <a name="delete-set"></a><span data-ttu-id="bbe7c-103">Удаление набора</span><span class="sxs-lookup"><span data-stu-id="bbe7c-103">Delete set</span></span>
<span data-ttu-id="bbe7c-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="bbe7c-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbe7c-105">Удаление объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="bbe7c-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbe7c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbe7c-106">Permissions</span></span>
<span data-ttu-id="bbe7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbe7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbe7c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbe7c-109">Permission type</span></span>|<span data-ttu-id="bbe7c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbe7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbe7c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbe7c-111">Delegated (work or school account)</span></span> |<span data-ttu-id="bbe7c-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbe7c-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="bbe7c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbe7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbe7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbe7c-114">Not supported.</span></span>    |
|<span data-ttu-id="bbe7c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbe7c-115">Application</span></span> | <span data-ttu-id="bbe7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbe7c-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="bbe7c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbe7c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="bbe7c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbe7c-118">Request headers</span></span>
|<span data-ttu-id="bbe7c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bbe7c-119">Name</span></span>|<span data-ttu-id="bbe7c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bbe7c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bbe7c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbe7c-121">Authorization</span></span>|<span data-ttu-id="bbe7c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbe7c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbe7c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbe7c-124">Request body</span></span>
<span data-ttu-id="bbe7c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbe7c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbe7c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbe7c-126">Response</span></span>

<span data-ttu-id="bbe7c-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bbe7c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bbe7c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="bbe7c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bbe7c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbe7c-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```


### <a name="response"></a><span data-ttu-id="bbe7c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbe7c-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->
