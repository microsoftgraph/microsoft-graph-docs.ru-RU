---
title: Удаление Екстерналграуп
description: Удаляет объект Екстерналграуп.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 4358c162e8ba07690c5bf19a11656ffcf292939e
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193948"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="8c254-103">Удаление Екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="8c254-103">Delete externalGroup</span></span>

<span data-ttu-id="8c254-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c254-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c254-105">Удаление объекта [екстерналграуп](../resources/externalgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8c254-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c254-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c254-106">Permissions</span></span>

<span data-ttu-id="8c254-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c254-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c254-109">Permission type</span></span>                        | <span data-ttu-id="8c254-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c254-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c254-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c254-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c254-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8c254-112">Not supported</span></span>                               |
| <span data-ttu-id="8c254-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c254-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c254-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8c254-114">Not supported</span></span>                               |
| <span data-ttu-id="8c254-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c254-115">Application</span></span>                            | <span data-ttu-id="8c254-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c254-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="8c254-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c254-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="8c254-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c254-118">Request headers</span></span>

| <span data-ttu-id="8c254-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8c254-119">Name</span></span>          | <span data-ttu-id="8c254-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c254-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8c254-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c254-121">Authorization</span></span> | <span data-ttu-id="8c254-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c254-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c254-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c254-124">Request body</span></span>

<span data-ttu-id="8c254-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c254-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c254-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c254-126">Response</span></span>

<span data-ttu-id="8c254-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c254-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8c254-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c254-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c254-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c254-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8c254-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c254-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
