---
title: Удаление группы
description: Удаление объекта Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fff0ead7cb2122db73ca7093d1c16c24496d23bf
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539479"
---
# <a name="delete-groups"></a><span data-ttu-id="d521b-103">Удаление групп</span><span class="sxs-lookup"><span data-stu-id="d521b-103">Delete groups</span></span>
<span data-ttu-id="d521b-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d521b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d521b-105">Удаление объекта [группы](../resources/termstore-group.md) в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="d521b-105">Delete a [group](../resources/termstore-group.md) object in the term [store].</span></span>

## <a name="permissions"></a><span data-ttu-id="d521b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d521b-106">Permissions</span></span>
<span data-ttu-id="d521b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d521b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d521b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d521b-109">Permission type</span></span>|<span data-ttu-id="d521b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d521b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d521b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d521b-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d521b-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d521b-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d521b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d521b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d521b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d521b-114">Not supported.</span></span>    |
|<span data-ttu-id="d521b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d521b-115">Application</span></span> | <span data-ttu-id="d521b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d521b-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d521b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d521b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/groups/{groupId}
```

## <a name="request-headers"></a><span data-ttu-id="d521b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d521b-118">Request headers</span></span>
|<span data-ttu-id="d521b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d521b-119">Name</span></span>|<span data-ttu-id="d521b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d521b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d521b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d521b-121">Authorization</span></span>|<span data-ttu-id="d521b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d521b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d521b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d521b-124">Request body</span></span>
<span data-ttu-id="d521b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d521b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d521b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d521b-126">Response</span></span>

<span data-ttu-id="d521b-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d521b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d521b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d521b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d521b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d521b-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_from_store"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/groups/{groupId}
```


### <a name="response"></a><span data-ttu-id="d521b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d521b-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termGroup",
  "suppressions": [
  ]
}
-->
