---
title: Удаление термина
description: Удаление объекта Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e9af0729c07896a707c35b7cd3e4eb3e122e5e10
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539443"
---
# <a name="delete-term"></a><span data-ttu-id="afaa9-103">Удаление термина</span><span class="sxs-lookup"><span data-stu-id="afaa9-103">Delete term</span></span>
<span data-ttu-id="afaa9-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="afaa9-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afaa9-105">Удаление объекта [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="afaa9-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afaa9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afaa9-106">Permissions</span></span>
<span data-ttu-id="afaa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afaa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afaa9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afaa9-109">Permission type</span></span>|<span data-ttu-id="afaa9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="afaa9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afaa9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afaa9-111">Delegated (work or school account)</span></span> |<span data-ttu-id="afaa9-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afaa9-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="afaa9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afaa9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afaa9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afaa9-114">Not supported.</span></span>    |
|<span data-ttu-id="afaa9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afaa9-115">Application</span></span> | <span data-ttu-id="afaa9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afaa9-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="afaa9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afaa9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="afaa9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afaa9-118">Request headers</span></span>
|<span data-ttu-id="afaa9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="afaa9-119">Name</span></span>|<span data-ttu-id="afaa9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="afaa9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="afaa9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afaa9-121">Authorization</span></span>|<span data-ttu-id="afaa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afaa9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afaa9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afaa9-124">Request body</span></span>
<span data-ttu-id="afaa9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afaa9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afaa9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="afaa9-126">Response</span></span>

<span data-ttu-id="afaa9-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="afaa9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="afaa9-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="afaa9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afaa9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="afaa9-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```


### <a name="response"></a><span data-ttu-id="afaa9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="afaa9-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete term",
  "suppressions": [
  ]
}
-->
