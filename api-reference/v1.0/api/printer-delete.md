---
title: Удаление принтера
description: Удаление (незарегистрированного) принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2a1d1b91e5f3b68995a27021c0b2fc3eb39de939
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517937"
---
# <a name="delete-printer"></a><span data-ttu-id="a7b26-103">Удаление принтера</span><span class="sxs-lookup"><span data-stu-id="a7b26-103">Delete printer</span></span>
<span data-ttu-id="a7b26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7b26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a7b26-105">Удаление (незарегистрированного) [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="a7b26-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7b26-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7b26-106">Permissions</span></span>
<span data-ttu-id="a7b26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a7b26-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a7b26-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a7b26-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a7b26-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a7b26-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7b26-111">Permission type</span></span> | <span data-ttu-id="a7b26-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7b26-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a7b26-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7b26-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a7b26-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a7b26-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="a7b26-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7b26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7b26-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b26-116">Not Supported.</span></span>|
|<span data-ttu-id="a7b26-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7b26-117">Application</span></span>|<span data-ttu-id="a7b26-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7b26-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7b26-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7b26-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="a7b26-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7b26-120">Request headers</span></span>
|<span data-ttu-id="a7b26-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a7b26-121">Name</span></span>|<span data-ttu-id="a7b26-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a7b26-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a7b26-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7b26-123">Authorization</span></span>|<span data-ttu-id="a7b26-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7b26-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7b26-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7b26-126">Request body</span></span>
<span data-ttu-id="a7b26-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7b26-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7b26-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7b26-128">Response</span></span>

<span data-ttu-id="a7b26-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a7b26-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a7b26-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a7b26-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7b26-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7b26-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}
```


### <a name="response"></a><span data-ttu-id="a7b26-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7b26-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

