---
title: Добавление includedGroups
description: Добавление групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cb589432f3ac977775af33f49f2647ad8b03be75
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547473"
---
# <a name="add-includedgroups"></a><span data-ttu-id="76869-103">Добавление includedGroups</span><span class="sxs-lookup"><span data-stu-id="76869-103">Add includedGroups</span></span>

<span data-ttu-id="76869-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76869-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76869-105">Добавление групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="76869-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="76869-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76869-106">Permissions</span></span>
<span data-ttu-id="76869-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76869-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76869-109">Permission type</span></span>|<span data-ttu-id="76869-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76869-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76869-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76869-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76869-112">Policy.Read.All, Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76869-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="76869-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76869-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76869-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76869-114">Not supported.</span></span>|
|<span data-ttu-id="76869-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76869-115">Application</span></span> | <span data-ttu-id="76869-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76869-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76869-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76869-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /policies/mobileAppManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="76869-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76869-118">Request headers</span></span>
|<span data-ttu-id="76869-119">Имя</span><span class="sxs-lookup"><span data-stu-id="76869-119">Name</span></span>|<span data-ttu-id="76869-120">Описание</span><span class="sxs-lookup"><span data-stu-id="76869-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="76869-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76869-121">Authorization</span></span>|<span data-ttu-id="76869-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76869-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="76869-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76869-124">Content-Type</span></span>|<span data-ttu-id="76869-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76869-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76869-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76869-127">Request body</span></span>
<span data-ttu-id="76869-128">В теле запроса поставляют представление JSON [группового](../resources/group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="76869-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="76869-129">В следующей таблице показаны свойства, необходимые при добавлении [группы.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="76869-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="76869-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76869-130">Property</span></span>|<span data-ttu-id="76869-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76869-131">Type</span></span>|<span data-ttu-id="76869-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76869-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76869-133">id</span><span class="sxs-lookup"><span data-stu-id="76869-133">id</span></span>|<span data-ttu-id="76869-134">String</span><span class="sxs-lookup"><span data-stu-id="76869-134">String</span></span>|<span data-ttu-id="76869-135">Уникальный идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="76869-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="76869-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="76869-136">Response</span></span>

<span data-ttu-id="76869-137">При успешном выполнении этот метод возвращает код отклика `204 No Content` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="76869-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76869-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="76869-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76869-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="76869-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/$ref
Content-Type: application/json

{
  "@odata.id": "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"
}
```

### <a name="response"></a><span data-ttu-id="76869-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="76869-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
