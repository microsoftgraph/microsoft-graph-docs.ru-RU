---
title: Удаление mobileAppManagementPolicy
description: Удаление политики управления мобильными приложениями.
author: michaelrm97
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4676980ef37e8cf60410726ce018bb30287a58e0
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401698"
---
# <a name="delete-mobileappmanagementpolicy"></a><span data-ttu-id="68e94-103">Удаление mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="68e94-103">Delete mobileAppManagementPolicy</span></span>

<span data-ttu-id="68e94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e94-105">Удаление [объекта mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="68e94-105">Delete a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="68e94-106">Эта операция поддерживается только в том случае, если политика больше не действительна; то есть, если **свойство isValid** является ложным, что указывает на удаление основного объекта службы, связанного с приложением для этой политики.</span><span class="sxs-lookup"><span data-stu-id="68e94-106">This operation is only supported when the policy is no longer valid; that is, when the **isValid** property is false, which indicates that the service principal associated with the application for this policy has been deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="68e94-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68e94-107">Permissions</span></span>

<span data-ttu-id="68e94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e94-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68e94-110">Permission type</span></span>|<span data-ttu-id="68e94-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68e94-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68e94-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68e94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68e94-113">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="68e94-113">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="68e94-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68e94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e94-115">Not supported.</span></span>|
|<span data-ttu-id="68e94-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68e94-116">Application</span></span> | <span data-ttu-id="68e94-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68e94-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68e94-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68e94-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68e94-119">Request headers</span></span>

|<span data-ttu-id="68e94-120">Имя</span><span class="sxs-lookup"><span data-stu-id="68e94-120">Name</span></span>|<span data-ttu-id="68e94-121">Описание</span><span class="sxs-lookup"><span data-stu-id="68e94-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68e94-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68e94-122">Authorization</span></span>|<span data-ttu-id="68e94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68e94-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68e94-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68e94-125">Request body</span></span>

<span data-ttu-id="68e94-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68e94-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68e94-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e94-127">Response</span></span>

<span data-ttu-id="68e94-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68e94-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68e94-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="68e94-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68e94-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="68e94-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_mobilitymanagementpolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="68e94-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e94-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
