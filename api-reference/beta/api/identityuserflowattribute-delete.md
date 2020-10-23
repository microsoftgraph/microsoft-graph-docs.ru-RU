---
title: Удаление Идентитюсерфловаттрибуте
description: Удаление Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 76eaa73ad22a2e418caf9bff7904422c16c01037
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742406"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="a3f6b-103">Удаление Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="a3f6b-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="a3f6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3f6b-105">Удаление [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="a3f6b-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="a3f6b-106">Удалить можно только настраиваемые атрибуты пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3f6b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3f6b-107">Permissions</span></span>

<span data-ttu-id="a3f6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3f6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3f6b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3f6b-110">Permission type</span></span>      | <span data-ttu-id="a3f6b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3f6b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3f6b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3f6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3f6b-113">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a3f6b-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a3f6b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3f6b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a3f6b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-115">Not supported.</span></span>|
|<span data-ttu-id="a3f6b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3f6b-116">Application</span></span>|<span data-ttu-id="a3f6b-117">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a3f6b-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="a3f6b-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a3f6b-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a3f6b-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a3f6b-119">Global administrator</span></span>
* <span data-ttu-id="a3f6b-120">Администратор атрибутов пользовательского процесса внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="a3f6b-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a3f6b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3f6b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a3f6b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3f6b-122">Request headers</span></span>

|<span data-ttu-id="a3f6b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a3f6b-123">Name</span></span>|<span data-ttu-id="a3f6b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a3f6b-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a3f6b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3f6b-125">Authorization</span></span>|<span data-ttu-id="a3f6b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3f6b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3f6b-128">Request body</span></span>

<span data-ttu-id="a3f6b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3f6b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3f6b-130">Response</span></span>

<span data-ttu-id="a3f6b-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3f6b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a3f6b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3f6b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3f6b-133">Request</span></span>

<span data-ttu-id="a3f6b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```

### <a name="response"></a><span data-ttu-id="a3f6b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3f6b-135">Response</span></span>

<span data-ttu-id="a3f6b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a3f6b-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
