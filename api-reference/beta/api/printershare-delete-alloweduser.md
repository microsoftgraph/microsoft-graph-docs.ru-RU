---
title: Удаление Алловедусер из Принтершаре
description: Отозвать доступ указанного пользователя, чтобы отправить задания печати на связанный общий принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b5a6c8028c84fa509e6cb21609ee105f0b29a1b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035542"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="116ae-103">Удаление Алловедусер из Принтершаре</span><span class="sxs-lookup"><span data-stu-id="116ae-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="116ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="116ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="116ae-105">Отозвать доступ указанного пользователя, чтобы послать задания печати связанному [принтершаре](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="116ae-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="116ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="116ae-106">Permissions</span></span>
<span data-ttu-id="116ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="116ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="116ae-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="116ae-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="116ae-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="116ae-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="116ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="116ae-111">Permission type</span></span> | <span data-ttu-id="116ae-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="116ae-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="116ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="116ae-113">Delegated (work or school account)</span></span>| <span data-ttu-id="116ae-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="116ae-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="116ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="116ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="116ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="116ae-116">Not Supported.</span></span>|
|<span data-ttu-id="116ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="116ae-117">Application</span></span>|<span data-ttu-id="116ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="116ae-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="116ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="116ae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShare/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="116ae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="116ae-120">Request headers</span></span>
| <span data-ttu-id="116ae-121">Имя</span><span class="sxs-lookup"><span data-stu-id="116ae-121">Name</span></span>          | <span data-ttu-id="116ae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="116ae-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="116ae-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="116ae-123">Authorization</span></span> | <span data-ttu-id="116ae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="116ae-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="116ae-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="116ae-126">Request body</span></span>
<span data-ttu-id="116ae-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="116ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="116ae-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="116ae-128">Response</span></span>
<span data-ttu-id="116ae-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="116ae-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="116ae-131">Пример</span><span class="sxs-lookup"><span data-stu-id="116ae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="116ae-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="116ae-132">Request</span></span>
<span data-ttu-id="116ae-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="116ae-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShare/{id}/allowedUsers/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="116ae-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="116ae-134">Response</span></span>
<span data-ttu-id="116ae-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="116ae-135">The following is an example of the response.</span></span>
><span data-ttu-id="116ae-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="116ae-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


