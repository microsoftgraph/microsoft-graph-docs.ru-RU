---
title: Удаление mobileDeviceManagementPolicy
description: Удаление политики управления мобильными устройствами.
author: michaelrm97
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 800cec45f578e97286982303a0e81d5b16895098
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401692"
---
# <a name="delete-mobiledevicemanagementpolicy"></a><span data-ttu-id="03ef8-103">Удаление mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="03ef8-103">Delete mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="03ef8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03ef8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03ef8-105">Удаление [объекта mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="03ef8-105">Delete a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="03ef8-106">Эта операция поддерживается только в том случае, если политика больше не действительна; то есть, если **свойство isValid** является ложным, что указывает на удаление основного объекта службы, связанного с приложением для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03ef8-106">This operation is only supported when the policy is no longer valid; that is, when the **isValid** property is false, which indicates that the service principal associated with the application for this policy has been deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="03ef8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03ef8-107">Permissions</span></span>

<span data-ttu-id="03ef8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03ef8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03ef8-110">Permission type</span></span>|<span data-ttu-id="03ef8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03ef8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03ef8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03ef8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03ef8-113">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="03ef8-113">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="03ef8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03ef8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03ef8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ef8-115">Not supported.</span></span>|
|<span data-ttu-id="03ef8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03ef8-116">Application</span></span> | <span data-ttu-id="03ef8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03ef8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03ef8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03ef8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03ef8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03ef8-119">Request headers</span></span>

|<span data-ttu-id="03ef8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03ef8-120">Name</span></span>|<span data-ttu-id="03ef8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03ef8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03ef8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03ef8-122">Authorization</span></span>|<span data-ttu-id="03ef8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03ef8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ef8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03ef8-125">Request body</span></span>

<span data-ttu-id="03ef8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03ef8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03ef8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ef8-127">Response</span></span>

<span data-ttu-id="03ef8-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03ef8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03ef8-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="03ef8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03ef8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="03ef8-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_mobilitymanagementpolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="03ef8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="03ef8-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
