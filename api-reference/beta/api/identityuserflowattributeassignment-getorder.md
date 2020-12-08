---
title: 'Идентитюсерфловаттрибутеассигнмент: упорядочение'
description: Получение порядка Идентитюсерфловаттрибутеассигнментс, собранных в пользовательском движении.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653a1e83ee96418dc70129790f62ea764e6326f9
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581427"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="4886f-103">Идентитюсерфловаттрибутеассигнмент: упорядочение</span><span class="sxs-lookup"><span data-stu-id="4886f-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="4886f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4886f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4886f-105">Получение порядка Идентитюсерфловаттрибутеассигнментс, собранных в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="4886f-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="4886f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4886f-106">Permissions</span></span>

<span data-ttu-id="4886f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4886f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4886f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4886f-109">Permission type</span></span>|<span data-ttu-id="4886f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4886f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4886f-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4886f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4886f-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4886f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4886f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4886f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4886f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4886f-114">Not supported</span></span>|
|<span data-ttu-id="4886f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4886f-115">Application</span></span>|<span data-ttu-id="4886f-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4886f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4886f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4886f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/getOrder
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="4886f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4886f-118">Request headers</span></span>

|<span data-ttu-id="4886f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4886f-119">Name</span></span>|<span data-ttu-id="4886f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4886f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4886f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4886f-121">Authorization</span></span>|<span data-ttu-id="4886f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4886f-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="4886f-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4886f-124">Function parameters</span></span>

<span data-ttu-id="4886f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4886f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4886f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4886f-126">Response</span></span>

<span data-ttu-id="4886f-127">В случае успеха эта функция возвращает `200 OK` код отклика и объект [ассигнментордер](../resources/assignmentorder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4886f-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4886f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="4886f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4886f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4886f-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder
```

### <a name="response"></a><span data-ttu-id="4886f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4886f-130">Response</span></span>

<span data-ttu-id="4886f-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4886f-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta$metadata#microsoft.graph.assignmentOrder",
    "order": [
        "extension_GUID_ShoeSize",
        "City"
    ]
}
```
