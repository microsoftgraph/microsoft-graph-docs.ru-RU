---
title: Список включенGroups
description: Получите список групп, включенных в политику управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9f29a263601958820d69fe51f146d34eb5a079c6
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401465"
---
# <a name="list-includedgroups"></a><span data-ttu-id="3f74c-103">Список включенGroups</span><span class="sxs-lookup"><span data-stu-id="3f74c-103">List includedGroups</span></span>

<span data-ttu-id="3f74c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f74c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f74c-105">Получите список групп, включенных в политику управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="3f74c-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f74c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f74c-106">Permissions</span></span>

<span data-ttu-id="3f74c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f74c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f74c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f74c-109">Permission type</span></span>|<span data-ttu-id="3f74c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f74c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f74c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f74c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f74c-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="3f74c-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="3f74c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f74c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f74c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f74c-114">Not supported.</span></span>|
|<span data-ttu-id="3f74c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f74c-115">Application</span></span> | <span data-ttu-id="3f74c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f74c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f74c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f74c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="3f74c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f74c-118">Request headers</span></span>

|<span data-ttu-id="3f74c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3f74c-119">Name</span></span>|<span data-ttu-id="3f74c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3f74c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3f74c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f74c-121">Authorization</span></span>|<span data-ttu-id="3f74c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f74c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f74c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f74c-124">Request body</span></span>

<span data-ttu-id="3f74c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f74c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f74c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f74c-126">Response</span></span>

<span data-ttu-id="3f74c-127">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="3f74c-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f74c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f74c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f74c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f74c-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="3f74c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f74c-130">Response</span></span>

><span data-ttu-id="3f74c-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3f74c-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
