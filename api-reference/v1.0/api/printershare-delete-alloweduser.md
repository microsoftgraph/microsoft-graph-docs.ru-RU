---
title: Удаление allowedUser из printerShare
description: Отзовет доступ указанного пользователя к отправке заданий печати в связанную долю принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 540fea358367e6d0daa025ccc005df551ba151e2
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517571"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="ce802-103">Удаление allowedUser из printerShare</span><span class="sxs-lookup"><span data-stu-id="ce802-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="ce802-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce802-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="ce802-105">Отзовет доступ указанного пользователя для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="ce802-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce802-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce802-106">Permissions</span></span>
<span data-ttu-id="ce802-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ce802-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ce802-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="ce802-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="ce802-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ce802-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce802-111">Permission type</span></span> | <span data-ttu-id="ce802-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce802-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ce802-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce802-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ce802-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce802-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ce802-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce802-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce802-116">Not Supported.</span></span>|
|<span data-ttu-id="ce802-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce802-117">Application</span></span>|<span data-ttu-id="ce802-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce802-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce802-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce802-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShare/{printerShareId}/allowedUsers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ce802-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce802-120">Request headers</span></span>
| <span data-ttu-id="ce802-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ce802-121">Name</span></span>          | <span data-ttu-id="ce802-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ce802-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ce802-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce802-123">Authorization</span></span> | <span data-ttu-id="ce802-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce802-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce802-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce802-126">Request body</span></span>
<span data-ttu-id="ce802-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce802-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce802-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce802-128">Response</span></span>
<span data-ttu-id="ce802-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce802-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce802-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ce802-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce802-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce802-132">Request</span></span>
<span data-ttu-id="ce802-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce802-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/printerShare/{printerShareId}/allowedUsers/{userId}/$ref
```

### <a name="response"></a><span data-ttu-id="ce802-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce802-134">Response</span></span>
<span data-ttu-id="ce802-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce802-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
