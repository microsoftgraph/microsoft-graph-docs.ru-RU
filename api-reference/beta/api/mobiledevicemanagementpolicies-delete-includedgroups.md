---
title: Удаление includeGroup
description: Удаление группы из списка групп, включенных в политику управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5ae99d68109e361f90b62c8560c0093d50b8c226
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547713"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="a57b3-103">Delete includedGroup</span><span class="sxs-lookup"><span data-stu-id="a57b3-103">Delete includedGroup</span></span>

<span data-ttu-id="a57b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a57b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a57b3-105">Удаление группы из списка групп, включенных в политику управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="a57b3-105">Delete a group from the list of groups included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="a57b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a57b3-106">Permissions</span></span>

<span data-ttu-id="a57b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a57b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a57b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a57b3-109">Permission type</span></span>|<span data-ttu-id="a57b3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a57b3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a57b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a57b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a57b3-112">Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57b3-112">Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="a57b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a57b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a57b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57b3-114">Not supported.</span></span>|
|<span data-ttu-id="a57b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a57b3-115">Application</span></span> | <span data-ttu-id="a57b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57b3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a57b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a57b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a57b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a57b3-118">Request headers</span></span>

|<span data-ttu-id="a57b3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a57b3-119">Name</span></span>|<span data-ttu-id="a57b3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a57b3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a57b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a57b3-121">Authorization</span></span>|<span data-ttu-id="a57b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a57b3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a57b3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a57b3-124">Request body</span></span>

<span data-ttu-id="a57b3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a57b3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a57b3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a57b3-126">Response</span></span>

<span data-ttu-id="a57b3-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a57b3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a57b3-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="a57b3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a57b3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a57b3-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/$ref
```

### <a name="response"></a><span data-ttu-id="a57b3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a57b3-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
