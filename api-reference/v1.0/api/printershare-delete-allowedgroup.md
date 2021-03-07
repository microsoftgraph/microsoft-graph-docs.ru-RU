---
title: Удаление allowedGroup из принтераShare
description: Отзовет доступ указанной группы для отправки заданий печати в связанную долю принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 18e4ff248368cf79836797566ae6a8846d2c70d9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517572"
---
# <a name="delete-allowedgroup-from-printershare"></a><span data-ttu-id="47ab4-103">Удаление allowedGroup из принтераShare</span><span class="sxs-lookup"><span data-stu-id="47ab4-103">Delete allowedGroup from printerShare</span></span>

<span data-ttu-id="47ab4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47ab4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="47ab4-105">Отзовет доступ указанной группы для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="47ab4-105">Revoke the specified group's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="47ab4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47ab4-106">Permissions</span></span>
<span data-ttu-id="47ab4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47ab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="47ab4-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="47ab4-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="47ab4-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="47ab4-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="47ab4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47ab4-111">Permission type</span></span> | <span data-ttu-id="47ab4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47ab4-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="47ab4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47ab4-113">Delegated (work or school account)</span></span>| <span data-ttu-id="47ab4-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47ab4-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="47ab4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47ab4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47ab4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47ab4-116">Not Supported.</span></span>|
|<span data-ttu-id="47ab4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47ab4-117">Application</span></span>|<span data-ttu-id="47ab4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47ab4-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47ab4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47ab4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/shares/{printerShareId}/allowedGroups/{groupId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="47ab4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47ab4-120">Request headers</span></span>
| <span data-ttu-id="47ab4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="47ab4-121">Name</span></span>          | <span data-ttu-id="47ab4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="47ab4-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="47ab4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47ab4-123">Authorization</span></span> | <span data-ttu-id="47ab4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47ab4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47ab4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47ab4-126">Request body</span></span>
<span data-ttu-id="47ab4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47ab4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47ab4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="47ab4-128">Response</span></span>
<span data-ttu-id="47ab4-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47ab4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47ab4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="47ab4-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="47ab4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="47ab4-132">Request</span></span>
<span data-ttu-id="47ab4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47ab4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_allowedgroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups/{groupId}/$ref
```
### <a name="response"></a><span data-ttu-id="47ab4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="47ab4-134">Response</span></span>
<span data-ttu-id="47ab4-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47ab4-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

