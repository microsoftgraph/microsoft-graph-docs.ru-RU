---
title: Удаление Клаудпкпровисионингполици
description: Удаление объекта Клаудпкпровисионингполици.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4f85b29e0375c10f8e3bb9f1132bf7c9a8b0aafd
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378557"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="25ba1-103">Удаление Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="25ba1-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="25ba1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25ba1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25ba1-105">Удаление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="25ba1-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="25ba1-106">Вы не можете удалить используемую политику.</span><span class="sxs-lookup"><span data-stu-id="25ba1-106">You can’t delete a policy that’s in use.</span></span>

## <a name="permissions"></a><span data-ttu-id="25ba1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25ba1-107">Permissions</span></span>

<span data-ttu-id="25ba1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25ba1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ba1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25ba1-110">Permission type</span></span>|<span data-ttu-id="25ba1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25ba1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25ba1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25ba1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25ba1-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ba1-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="25ba1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25ba1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25ba1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25ba1-115">Not supported.</span></span>|
|<span data-ttu-id="25ba1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25ba1-116">Application</span></span>|<span data-ttu-id="25ba1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25ba1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25ba1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25ba1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="25ba1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25ba1-119">Request headers</span></span>

|<span data-ttu-id="25ba1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="25ba1-120">Name</span></span>|<span data-ttu-id="25ba1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="25ba1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="25ba1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25ba1-122">Authorization</span></span>|<span data-ttu-id="25ba1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25ba1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25ba1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25ba1-125">Request body</span></span>

<span data-ttu-id="25ba1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25ba1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25ba1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ba1-127">Response</span></span>

<span data-ttu-id="25ba1-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25ba1-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25ba1-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="25ba1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25ba1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="25ba1-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="25ba1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="25ba1-131">Response</span></span>

<span data-ttu-id="25ba1-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="25ba1-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
