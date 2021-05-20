---
title: Список включенGroups
description: Получите список групп, включенных в политику управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2b83a7c797d790600aa391712e1deb70b5639cf7
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547422"
---
# <a name="list-includedgroups"></a><span data-ttu-id="7d507-103">Список включенGroups</span><span class="sxs-lookup"><span data-stu-id="7d507-103">List includedGroups</span></span>

<span data-ttu-id="7d507-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d507-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d507-105">Получите список групп, включенных в политику управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="7d507-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d507-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d507-106">Permissions</span></span>

<span data-ttu-id="7d507-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d507-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d507-109">Permission type</span></span>|<span data-ttu-id="7d507-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d507-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d507-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d507-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d507-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d507-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="7d507-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d507-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d507-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d507-114">Not supported.</span></span>|
|<span data-ttu-id="7d507-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d507-115">Application</span></span> | <span data-ttu-id="7d507-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d507-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d507-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d507-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="7d507-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d507-118">Request headers</span></span>

|<span data-ttu-id="7d507-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d507-119">Name</span></span>|<span data-ttu-id="7d507-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d507-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7d507-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d507-121">Authorization</span></span>|<span data-ttu-id="7d507-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d507-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d507-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d507-124">Request body</span></span>

<span data-ttu-id="7d507-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d507-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d507-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d507-126">Response</span></span>

<span data-ttu-id="7d507-127">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="7d507-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d507-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d507-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d507-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d507-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="7d507-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d507-130">Response</span></span>

><span data-ttu-id="7d507-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d507-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef",
      "displayName": "Test MDM Group"
    }
  ]
}
```
