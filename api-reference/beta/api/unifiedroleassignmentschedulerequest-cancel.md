---
title: 'unifiedRoleAssignmentScheduleRequest: отмена'
description: Отмена единой системыRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 801e5aa26043a4291bdbacba7d99ca26d06245d8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299796"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a><span data-ttu-id="281a0-103">unifiedRoleAssignmentScheduleRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="281a0-103">unifiedRoleAssignmentScheduleRequest: cancel</span></span>
<span data-ttu-id="281a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="281a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="281a0-105">Немедленно [отмените унифицированныйRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и задайте системе автоматическое удаление отмененного запроса через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="281a0-105">Immediately cancel a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="281a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="281a0-106">Permissions</span></span>
<span data-ttu-id="281a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="281a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="281a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="281a0-109">Permission type</span></span>|<span data-ttu-id="281a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="281a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="281a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="281a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="281a0-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="281a0-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="281a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="281a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="281a0-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="281a0-114">Not supported</span></span>|
|<span data-ttu-id="281a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="281a0-115">Application</span></span>|<span data-ttu-id="281a0-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="281a0-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="281a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="281a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="281a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="281a0-118">Request headers</span></span>
|<span data-ttu-id="281a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="281a0-119">Name</span></span>|<span data-ttu-id="281a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="281a0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="281a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="281a0-121">Authorization</span></span>|<span data-ttu-id="281a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="281a0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="281a0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="281a0-124">Request body</span></span>
<span data-ttu-id="281a0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="281a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="281a0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="281a0-126">Response</span></span>

<span data-ttu-id="281a0-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="281a0-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="281a0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="281a0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="281a0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="281a0-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```


### <a name="response"></a><span data-ttu-id="281a0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="281a0-130">Response</span></span>
<span data-ttu-id="281a0-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="281a0-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

