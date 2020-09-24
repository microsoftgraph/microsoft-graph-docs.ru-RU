---
title: Создание группы
description: Создание нового объекта Group.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 314795b1edad398a093b3c1bbfc401c0ef450c23
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258452"
---
# <a name="create-group"></a><span data-ttu-id="9505e-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="9505e-103">Create group</span></span>
<span data-ttu-id="9505e-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="9505e-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9505e-105">Создание нового объекта [Group](../resources/termstore-group.md) .</span><span class="sxs-lookup"><span data-stu-id="9505e-105">Create a new [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9505e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9505e-106">Permissions</span></span>
<span data-ttu-id="9505e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9505e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9505e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9505e-109">Permission type</span></span>|<span data-ttu-id="9505e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9505e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9505e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9505e-111">Delegated (work or school account)</span></span> |<span data-ttu-id="9505e-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9505e-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="9505e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9505e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9505e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9505e-114">Not supported.</span></span>    |
|<span data-ttu-id="9505e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9505e-115">Application</span></span> | <span data-ttu-id="9505e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9505e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9505e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9505e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /termStore/groups
```

## <a name="request-headers"></a><span data-ttu-id="9505e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9505e-118">Request headers</span></span>
|<span data-ttu-id="9505e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9505e-119">Name</span></span>|<span data-ttu-id="9505e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9505e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9505e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9505e-121">Authorization</span></span>|<span data-ttu-id="9505e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9505e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9505e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9505e-124">Content-Type</span></span>|<span data-ttu-id="9505e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9505e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9505e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9505e-127">Request body</span></span>
<span data-ttu-id="9505e-128">В тексте запроса добавьте представление объекта [Group](../resources/termstore-group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9505e-128">In the request body, supply a JSON representation of the [group](../resources/termstore-group.md) object.</span></span>

<span data-ttu-id="9505e-129">В следующей таблице приведены свойства, необходимые при создании [группы](../resources/termstore-group.md).</span><span class="sxs-lookup"><span data-stu-id="9505e-129">The following table shows the properties that are required when you create the [group](../resources/termstore-group.md).</span></span>

|<span data-ttu-id="9505e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9505e-130">Property</span></span>|<span data-ttu-id="9505e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9505e-131">Type</span></span>|<span data-ttu-id="9505e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9505e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9505e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9505e-133">displayName</span></span>|<span data-ttu-id="9505e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9505e-134">String</span></span>|<span data-ttu-id="9505e-135">Имя создаваемой группы.</span><span class="sxs-lookup"><span data-stu-id="9505e-135">Name of the group to be created.</span></span>|



## <a name="response"></a><span data-ttu-id="9505e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9505e-136">Response</span></span>

<span data-ttu-id="9505e-137">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/termstore-group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9505e-137">If successful, this method returns a `201 Created` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9505e-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="9505e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9505e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9505e-139">Request</span></span>
<!-- {
  "blockType": "request",
  "displayName": "myGroup"
}-->

``` http
POST https://graph.microsoft.com/beta/termStore/groups
Content-Type: application/json
Content-length: 135

{
  "displayName" : "myGroup"
}
```


### <a name="response"></a><span data-ttu-id="9505e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9505e-140">Response</span></span>
<span data-ttu-id="9505e-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9505e-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "85825593-5593-8582-9355-828593558285",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "displayName": "myGroup"  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termGroup",
  "suppressions": [
  ]
}
-->


