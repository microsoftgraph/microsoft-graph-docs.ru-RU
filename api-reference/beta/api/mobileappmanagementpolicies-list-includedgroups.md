---
title: Список включенGroups
description: Получите список групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 26cbec0d2fe976045a320a80fe3a69a53fbc74f6
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401668"
---
# <a name="list-includedgroups"></a><span data-ttu-id="e2973-103">Список включенGroups</span><span class="sxs-lookup"><span data-stu-id="e2973-103">List includedGroups</span></span>

<span data-ttu-id="e2973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2973-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2973-105">Получите список групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="e2973-105">Get the list of groups that are included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2973-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2973-106">Permissions</span></span>

<span data-ttu-id="e2973-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2973-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2973-109">Permission type</span></span>|<span data-ttu-id="e2973-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2973-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2973-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2973-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2973-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="e2973-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="e2973-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2973-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2973-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2973-114">Not supported.</span></span>|
|<span data-ttu-id="e2973-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2973-115">Application</span></span> | <span data-ttu-id="e2973-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2973-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2973-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2973-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="e2973-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2973-118">Request headers</span></span>

|<span data-ttu-id="e2973-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e2973-119">Name</span></span>|<span data-ttu-id="e2973-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2973-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e2973-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2973-121">Authorization</span></span>|<span data-ttu-id="e2973-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2973-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2973-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2973-124">Request body</span></span>

<span data-ttu-id="e2973-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2973-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2973-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2973-126">Response</span></span>

<span data-ttu-id="e2973-127">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="e2973-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2973-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e2973-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2973-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2973-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="e2973-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2973-130">Response</span></span>

><span data-ttu-id="e2973-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e2973-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
