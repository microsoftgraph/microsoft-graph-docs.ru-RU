---
title: Добавление includedGroups
description: Добавление групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cce0d4d98ca36506297780f424f371ca31b3e5d0
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401430"
---
# <a name="add-includedgroups"></a><span data-ttu-id="04b8a-103">Добавление includedGroups</span><span class="sxs-lookup"><span data-stu-id="04b8a-103">Add includedGroups</span></span>

<span data-ttu-id="04b8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04b8a-105">Добавление групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="04b8a-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="04b8a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04b8a-106">Permissions</span></span>

<span data-ttu-id="04b8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b8a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b8a-109">Permission type</span></span>|<span data-ttu-id="04b8a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b8a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b8a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b8a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04b8a-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="04b8a-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="04b8a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b8a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b8a-114">Not supported.</span></span>|
|<span data-ttu-id="04b8a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04b8a-115">Application</span></span> | <span data-ttu-id="04b8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b8a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b8a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b8a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /policies/mobileDeviceManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="04b8a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b8a-118">Request headers</span></span>
|<span data-ttu-id="04b8a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="04b8a-119">Name</span></span>|<span data-ttu-id="04b8a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="04b8a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04b8a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b8a-121">Authorization</span></span>|<span data-ttu-id="04b8a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b8a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04b8a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04b8a-124">Content-Type</span></span>|<span data-ttu-id="04b8a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04b8a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b8a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b8a-127">Request body</span></span>
<span data-ttu-id="04b8a-128">В теле запроса поставляют представление JSON [группового](../resources/group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="04b8a-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="04b8a-129">В следующей таблице показаны свойства, необходимые при добавлении [группы.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="04b8a-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="04b8a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04b8a-130">Property</span></span>|<span data-ttu-id="04b8a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04b8a-131">Type</span></span>|<span data-ttu-id="04b8a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04b8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b8a-133">id</span><span class="sxs-lookup"><span data-stu-id="04b8a-133">id</span></span>|<span data-ttu-id="04b8a-134">String</span><span class="sxs-lookup"><span data-stu-id="04b8a-134">String</span></span>|<span data-ttu-id="04b8a-135">Уникальный идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="04b8a-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="04b8a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b8a-136">Response</span></span>

<span data-ttu-id="04b8a-137">При успешном выполнении этот метод возвращает код отклика `204 No Content` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04b8a-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04b8a-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="04b8a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04b8a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b8a-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/includedGroups/$ref
Content-Type: application/json

{
  "@odata.id": "https://graph.microsoft.com/odata/groups('dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef')"
}
```

### <a name="response"></a><span data-ttu-id="04b8a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b8a-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
