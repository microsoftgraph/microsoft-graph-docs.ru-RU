---
title: Добавление includedGroups
description: Добавление групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3ec6ddda47493892c698c210dd0408f0cd1dfb27
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401654"
---
# <a name="add-includedgroups"></a><span data-ttu-id="8bf4b-103">Добавление includedGroups</span><span class="sxs-lookup"><span data-stu-id="8bf4b-103">Add includedGroups</span></span>

<span data-ttu-id="8bf4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bf4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bf4b-105">Добавление групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bf4b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bf4b-106">Permissions</span></span>
<span data-ttu-id="8bf4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf4b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bf4b-109">Permission type</span></span>|<span data-ttu-id="8bf4b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bf4b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bf4b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bf4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8bf4b-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="8bf4b-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="8bf4b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bf4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bf4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-114">Not supported.</span></span>|
|<span data-ttu-id="8bf4b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bf4b-115">Application</span></span> | <span data-ttu-id="8bf4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bf4b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bf4b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /policies/mobileAppManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8bf4b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bf4b-118">Request headers</span></span>
|<span data-ttu-id="8bf4b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8bf4b-119">Name</span></span>|<span data-ttu-id="8bf4b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf4b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8bf4b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bf4b-121">Authorization</span></span>|<span data-ttu-id="8bf4b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8bf4b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bf4b-124">Content-Type</span></span>|<span data-ttu-id="8bf4b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bf4b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bf4b-127">Request body</span></span>
<span data-ttu-id="8bf4b-128">В теле запроса поставляют представление JSON [группового](../resources/group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="8bf4b-129">В следующей таблице показаны свойства, необходимые при добавлении [группы.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="8bf4b-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="8bf4b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bf4b-130">Property</span></span>|<span data-ttu-id="8bf4b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8bf4b-131">Type</span></span>|<span data-ttu-id="8bf4b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bf4b-133">id</span><span class="sxs-lookup"><span data-stu-id="8bf4b-133">id</span></span>|<span data-ttu-id="8bf4b-134">String</span><span class="sxs-lookup"><span data-stu-id="8bf4b-134">String</span></span>|<span data-ttu-id="8bf4b-135">Уникальный идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="8bf4b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bf4b-136">Response</span></span>

<span data-ttu-id="8bf4b-137">При успешном выполнении этот метод возвращает код отклика `204 No Content` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8bf4b-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bf4b-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="8bf4b-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bf4b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bf4b-139">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="8bf4b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bf4b-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
