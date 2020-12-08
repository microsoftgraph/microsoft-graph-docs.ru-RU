---
title: Удаление Усераттрибутеассигнмент
description: Удаление объекта Идентитюсерфловаттрибутеассигнмент.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ea4c9ef7d2d9318c8b39b22dbdb72e43890d7dc2
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581431"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="641e2-103">Удаление Усераттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="641e2-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="641e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="641e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="641e2-105">Удаление объекта [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="641e2-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="641e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="641e2-106">Permissions</span></span>

<span data-ttu-id="641e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="641e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="641e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="641e2-109">Permission type</span></span>|<span data-ttu-id="641e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="641e2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="641e2-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="641e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="641e2-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="641e2-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="641e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="641e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="641e2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="641e2-114">Not supported</span></span>|
|<span data-ttu-id="641e2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="641e2-115">Application</span></span>|<span data-ttu-id="641e2-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="641e2-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="641e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="641e2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="641e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="641e2-118">Request headers</span></span>

|<span data-ttu-id="641e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="641e2-119">Name</span></span>|<span data-ttu-id="641e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="641e2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="641e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="641e2-121">Authorization</span></span>|<span data-ttu-id="641e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="641e2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="641e2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="641e2-124">Request body</span></span>

<span data-ttu-id="641e2-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="641e2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="641e2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="641e2-126">Response</span></span>

<span data-ttu-id="641e2-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="641e2-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="641e2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="641e2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="641e2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="641e2-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="641e2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="641e2-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
