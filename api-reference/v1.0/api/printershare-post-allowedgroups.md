---
title: Создание allowedGroup для принтераShare
description: Предоставление указанной группе доступа для отправки заданий печати на связанный принтер.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8db8facb302863ec96107c333b8e17f59f2b27a4
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573861"
---
# <a name="create-allowedgroup-for-printershare"></a><span data-ttu-id="2d114-103">Создание allowedGroup для принтераShare</span><span class="sxs-lookup"><span data-stu-id="2d114-103">Create allowedGroup for printerShare</span></span>
<span data-ttu-id="2d114-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d114-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2d114-105">Предоставление указанной группе доступа для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="2d114-105">Grant the specified group access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d114-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d114-106">Permissions</span></span>
<span data-ttu-id="2d114-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2d114-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2d114-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2d114-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="2d114-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2d114-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d114-111">Permission type</span></span> | <span data-ttu-id="2d114-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d114-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2d114-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d114-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2d114-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d114-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="2d114-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d114-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d114-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d114-116">Not Supported.</span></span>|
|<span data-ttu-id="2d114-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2d114-117">Application</span></span>|<span data-ttu-id="2d114-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d114-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d114-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d114-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/shares/{printerShareId}/allowedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2d114-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d114-120">Request headers</span></span>
|<span data-ttu-id="2d114-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2d114-121">Name</span></span>|<span data-ttu-id="2d114-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d114-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d114-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d114-123">Authorization</span></span>|<span data-ttu-id="2d114-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d114-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d114-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d114-126">Content-Type</span></span>|<span data-ttu-id="2d114-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d114-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d114-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d114-129">Request body</span></span>
<span data-ttu-id="2d114-130">В теле запроса укажи ссылку на объект группы с помощью формата, как показано `@odata.id` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="2d114-130">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="2d114-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d114-131">Response</span></span>

<span data-ttu-id="2d114-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2d114-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2d114-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d114-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d114-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d114-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/$ref
Content-Type: application/json
Content-length: 47

{
  "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}"
}
```


### <a name="response"></a><span data-ttu-id="2d114-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d114-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
}
-->
``` http
HTTP/1.1 204 No Content
```

