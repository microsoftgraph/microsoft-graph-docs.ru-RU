---
title: 'unifiedRoleEligibilityScheduleRequest: отмена'
description: Отмена единойRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 94e3fd5c5f42b5fc35a27724e77d47b07a7876ec
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299815"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="6819a-103">unifiedRoleEligibilityScheduleRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="6819a-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="6819a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6819a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6819a-105">Немедленно отмените [унифицированныйRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и заключите автоматическое удаление отмененного запроса через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="6819a-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="6819a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6819a-106">Permissions</span></span>
<span data-ttu-id="6819a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6819a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6819a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6819a-109">Permission type</span></span>|<span data-ttu-id="6819a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6819a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6819a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6819a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6819a-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6819a-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="6819a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6819a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6819a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6819a-114">Not supported</span></span>|
|<span data-ttu-id="6819a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6819a-115">Application</span></span>|<span data-ttu-id="6819a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6819a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6819a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6819a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="6819a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6819a-118">Request headers</span></span>
|<span data-ttu-id="6819a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6819a-119">Name</span></span>|<span data-ttu-id="6819a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6819a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6819a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6819a-121">Authorization</span></span>|<span data-ttu-id="6819a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6819a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6819a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6819a-124">Request body</span></span>
<span data-ttu-id="6819a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6819a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6819a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6819a-126">Response</span></span>

<span data-ttu-id="6819a-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6819a-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6819a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6819a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6819a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6819a-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```


### <a name="response"></a><span data-ttu-id="6819a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6819a-130">Response</span></span>
<span data-ttu-id="6819a-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6819a-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

