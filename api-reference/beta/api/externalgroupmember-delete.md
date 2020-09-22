---
title: Удаление Екстерналграупмембер
description: Удаление объекта Екстерналграупмембер.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 3347b51ba6b3fa5928e08ea85540cc0e634a1a7a
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193947"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="a7dbb-103">Удаление Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="a7dbb-103">Delete externalGroupMember</span></span>

<span data-ttu-id="a7dbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7dbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7dbb-105">Удаление объекта [екстерналграупмембер](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="a7dbb-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7dbb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7dbb-106">Permissions</span></span>

<span data-ttu-id="a7dbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7dbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7dbb-109">Permission type</span></span>                        | <span data-ttu-id="a7dbb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7dbb-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a7dbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7dbb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7dbb-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a7dbb-112">Not supported</span></span>                               |
| <span data-ttu-id="a7dbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7dbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7dbb-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a7dbb-114">Not supported</span></span>                               |
| <span data-ttu-id="a7dbb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7dbb-115">Application</span></span>                            | <span data-ttu-id="a7dbb-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7dbb-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="a7dbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7dbb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="a7dbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7dbb-118">Request headers</span></span>

| <span data-ttu-id="a7dbb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a7dbb-119">Name</span></span>          | <span data-ttu-id="a7dbb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a7dbb-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a7dbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7dbb-121">Authorization</span></span> | <span data-ttu-id="a7dbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7dbb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7dbb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7dbb-124">Request body</span></span>

<span data-ttu-id="a7dbb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7dbb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7dbb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7dbb-126">Response</span></span>

<span data-ttu-id="a7dbb-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7dbb-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a7dbb-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a7dbb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7dbb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7dbb-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="a7dbb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7dbb-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
