---
title: 'Хранитель: Activated'
description: Повторно активируйте хранитель в случае.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 40ac381da15065a4363471ba9c82c19080b84884
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597766"
---
# <a name="custodian-activate"></a><span data-ttu-id="75504-103">Хранитель: Activated</span><span class="sxs-lookup"><span data-stu-id="75504-103">custodian: activate</span></span>

<span data-ttu-id="75504-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75504-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75504-105">Активируйте хранитель, выпущенный из случая, чтобы сделать их частью этого случая.</span><span class="sxs-lookup"><span data-stu-id="75504-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="75504-106">Дополнительные сведения: [Управление custodians в расширенном случае обнаружения электронных](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian)данных.</span><span class="sxs-lookup"><span data-stu-id="75504-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="75504-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75504-107">Permissions</span></span>

<span data-ttu-id="75504-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75504-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75504-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75504-110">Permission type</span></span>|<span data-ttu-id="75504-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75504-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75504-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75504-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75504-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="75504-113">User.Read</span></span>|
|<span data-ttu-id="75504-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75504-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75504-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75504-115">Not supported.</span></span>|
|<span data-ttu-id="75504-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75504-116">Application</span></span>|<span data-ttu-id="75504-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75504-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75504-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75504-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="75504-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75504-119">Request headers</span></span>

|<span data-ttu-id="75504-120">Имя</span><span class="sxs-lookup"><span data-stu-id="75504-120">Name</span></span>|<span data-ttu-id="75504-121">Описание</span><span class="sxs-lookup"><span data-stu-id="75504-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75504-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75504-122">Authorization</span></span>|<span data-ttu-id="75504-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75504-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75504-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75504-125">Content-Type</span></span>|<span data-ttu-id="75504-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75504-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75504-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75504-128">Request body</span></span>

<span data-ttu-id="75504-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75504-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75504-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="75504-130">Response</span></span>

<span data-ttu-id="75504-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="75504-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="75504-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="75504-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75504-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="75504-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```

### <a name="response"></a><span data-ttu-id="75504-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="75504-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
