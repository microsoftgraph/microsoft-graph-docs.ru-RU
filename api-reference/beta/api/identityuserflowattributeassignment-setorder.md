---
title: 'Идентитюсерфловаттрибутеассигнмент: Сетордер'
description: Задайте порядок Идентитюсерфловаттрибутеассигнментс, собираемых в рамках пользовательского процесса.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 705acf8e65d7d01c40d98860c6f5066121d23a81
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581428"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="88948-103">Идентитюсерфловаттрибутеассигнмент: Сетордер</span><span class="sxs-lookup"><span data-stu-id="88948-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="88948-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88948-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88948-105">Задайте порядок Идентитюсерфловаттрибутеассигнментс, собираемых в рамках пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="88948-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="88948-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88948-106">Permissions</span></span>

<span data-ttu-id="88948-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88948-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88948-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88948-109">Permission type</span></span>|<span data-ttu-id="88948-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88948-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88948-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88948-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88948-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="88948-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="88948-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88948-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88948-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="88948-114">Not supported</span></span>|
|<span data-ttu-id="88948-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="88948-115">Application</span></span>|<span data-ttu-id="88948-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="88948-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88948-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88948-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="88948-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88948-118">Request headers</span></span>

|<span data-ttu-id="88948-119">Имя</span><span class="sxs-lookup"><span data-stu-id="88948-119">Name</span></span>|<span data-ttu-id="88948-120">Описание</span><span class="sxs-lookup"><span data-stu-id="88948-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88948-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88948-121">Authorization</span></span>|<span data-ttu-id="88948-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88948-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88948-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88948-124">Content-Type</span></span>|<span data-ttu-id="88948-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88948-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88948-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88948-127">Request body</span></span>

<span data-ttu-id="88948-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88948-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="88948-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="88948-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="88948-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="88948-130">Parameter</span></span>|<span data-ttu-id="88948-131">Тип</span><span class="sxs-lookup"><span data-stu-id="88948-131">Type</span></span>|<span data-ttu-id="88948-132">Описание</span><span class="sxs-lookup"><span data-stu-id="88948-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88948-133">невассигнментордер</span><span class="sxs-lookup"><span data-stu-id="88948-133">newAssignmentOrder</span></span>|[<span data-ttu-id="88948-134">ассигнментордер</span><span class="sxs-lookup"><span data-stu-id="88948-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="88948-135">Используется для определения порядка атрибутов, собранных в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="88948-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="88948-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="88948-136">Response</span></span>

<span data-ttu-id="88948-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88948-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="88948-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="88948-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88948-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="88948-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder

Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="88948-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="88948-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
