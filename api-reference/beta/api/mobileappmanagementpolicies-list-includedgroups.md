---
title: Список включенGroups
description: Получите список групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8c7af8b03a42050b423dd4533ae28a432523a907
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547494"
---
# <a name="list-includedgroups"></a><span data-ttu-id="fc365-103">Список включенGroups</span><span class="sxs-lookup"><span data-stu-id="fc365-103">List includedGroups</span></span>

<span data-ttu-id="fc365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc365-105">Получите список групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="fc365-105">Get the list of groups that are included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc365-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc365-106">Permissions</span></span>

<span data-ttu-id="fc365-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc365-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc365-109">Permission type</span></span>|<span data-ttu-id="fc365-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc365-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc365-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc365-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc365-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc365-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="fc365-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc365-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc365-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc365-114">Not supported.</span></span>|
|<span data-ttu-id="fc365-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc365-115">Application</span></span> | <span data-ttu-id="fc365-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc365-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc365-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc365-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="fc365-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc365-118">Request headers</span></span>

|<span data-ttu-id="fc365-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fc365-119">Name</span></span>|<span data-ttu-id="fc365-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc365-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fc365-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc365-121">Authorization</span></span>|<span data-ttu-id="fc365-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc365-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc365-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc365-124">Request body</span></span>

<span data-ttu-id="fc365-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc365-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc365-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc365-126">Response</span></span>

<span data-ttu-id="fc365-127">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="fc365-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc365-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc365-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc365-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc365-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPoliciesab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="fc365-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc365-130">Response</span></span>

><span data-ttu-id="fc365-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc365-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
      "displayName": "Test Group"
    }
  ]
}
```
