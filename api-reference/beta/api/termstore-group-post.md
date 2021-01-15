---
title: Создание группы
description: Создание объекта группы.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: bc7959ec7606a450e9ef920cd96b2550923b03f2
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873908"
---
# <a name="create-group"></a><span data-ttu-id="0b173-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="0b173-103">Create group</span></span>
<span data-ttu-id="0b173-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="0b173-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b173-105">Создание объекта [группы.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="0b173-105">Create a new [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b173-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b173-106">Permissions</span></span>
<span data-ttu-id="0b173-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b173-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b173-109">Permission type</span></span>|<span data-ttu-id="0b173-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b173-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b173-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b173-111">Delegated (work or school account)</span></span> |<span data-ttu-id="0b173-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b173-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="0b173-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b173-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b173-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b173-114">Not supported.</span></span>    |
|<span data-ttu-id="0b173-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b173-115">Application</span></span> | <span data-ttu-id="0b173-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b173-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b173-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b173-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /termStore/groups
```

## <a name="request-headers"></a><span data-ttu-id="0b173-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b173-118">Request headers</span></span>
|<span data-ttu-id="0b173-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b173-119">Name</span></span>|<span data-ttu-id="0b173-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0b173-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b173-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b173-121">Authorization</span></span>|<span data-ttu-id="0b173-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b173-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0b173-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b173-124">Content-Type</span></span>|<span data-ttu-id="0b173-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b173-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b173-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b173-127">Request body</span></span>
<span data-ttu-id="0b173-128">В теле запроса укажу представление объекта группы в [JSON.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="0b173-128">In the request body, supply a JSON representation of the [group](../resources/termstore-group.md) object.</span></span>

<span data-ttu-id="0b173-129">В следующей таблице показаны свойства, необходимые при создании [группы.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="0b173-129">The following table shows the properties that are required when you create the [group](../resources/termstore-group.md).</span></span>

|<span data-ttu-id="0b173-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b173-130">Property</span></span>|<span data-ttu-id="0b173-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b173-131">Type</span></span>|<span data-ttu-id="0b173-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b173-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b173-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0b173-133">displayName</span></span>|<span data-ttu-id="0b173-134">String</span><span class="sxs-lookup"><span data-stu-id="0b173-134">String</span></span>|<span data-ttu-id="0b173-135">Имя создаемой группы.</span><span class="sxs-lookup"><span data-stu-id="0b173-135">Name of the group to be created.</span></span>|



## <a name="response"></a><span data-ttu-id="0b173-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b173-136">Response</span></span>

<span data-ttu-id="0b173-137">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/termstore-group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b173-137">If successful, this method returns a `201 Created` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b173-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b173-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b173-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b173-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="0b173-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b173-140">Response</span></span>
<span data-ttu-id="0b173-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b173-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


