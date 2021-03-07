---
title: Удаление printConnector
description: Удаление (отрегистрации) printConnector.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4366aa9f3ab674861c404a4ce0f9c329a06b23e9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517476"
---
# <a name="delete-printconnector"></a><span data-ttu-id="de83d-103">Удаление printConnector</span><span class="sxs-lookup"><span data-stu-id="de83d-103">Delete printConnector</span></span>
<span data-ttu-id="de83d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de83d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="de83d-105">Удаление (незарегистрированного) **printConnector**.</span><span class="sxs-lookup"><span data-stu-id="de83d-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="de83d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de83d-106">Permissions</span></span>
<span data-ttu-id="de83d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de83d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="de83d-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="de83d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="de83d-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="de83d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="de83d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de83d-111">Permission type</span></span> | <span data-ttu-id="de83d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de83d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="de83d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de83d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="de83d-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de83d-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="de83d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de83d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de83d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de83d-116">Not Supported.</span></span>|
|<span data-ttu-id="de83d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="de83d-117">Application</span></span>|<span data-ttu-id="de83d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de83d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de83d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de83d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="de83d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de83d-120">Request headers</span></span>
|<span data-ttu-id="de83d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="de83d-121">Name</span></span>|<span data-ttu-id="de83d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="de83d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de83d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de83d-123">Authorization</span></span>|<span data-ttu-id="de83d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de83d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de83d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de83d-126">Request body</span></span>
<span data-ttu-id="de83d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de83d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de83d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="de83d-128">Response</span></span>
<span data-ttu-id="de83d-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="de83d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="de83d-131">Условия ошибки и сообщения</span><span class="sxs-lookup"><span data-stu-id="de83d-131">Error conditions and messages</span></span>

|<span data-ttu-id="de83d-132">Сценарий</span><span class="sxs-lookup"><span data-stu-id="de83d-132">Scenario</span></span>|<span data-ttu-id="de83d-133">Method</span><span class="sxs-lookup"><span data-stu-id="de83d-133">Method</span></span>|<span data-ttu-id="de83d-134">Код</span><span class="sxs-lookup"><span data-stu-id="de83d-134">Code</span></span>|<span data-ttu-id="de83d-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="de83d-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="de83d-136">Пользователь пытается удалить соединителя, который имеет один или несколько принтеров зарегистрированы</span><span class="sxs-lookup"><span data-stu-id="de83d-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="de83d-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="de83d-137">DELETE</span></span>|<span data-ttu-id="de83d-138">409</span><span class="sxs-lookup"><span data-stu-id="de83d-138">409</span></span>|<span data-ttu-id="de83d-139">Перед удалением соединителя удаляйте связанные принтеры.</span><span class="sxs-lookup"><span data-stu-id="de83d-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="examples"></a><span data-ttu-id="de83d-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="de83d-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de83d-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="de83d-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printconnector"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```


### <a name="response"></a><span data-ttu-id="de83d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="de83d-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

